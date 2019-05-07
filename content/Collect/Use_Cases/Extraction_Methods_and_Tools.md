+++
title = 'Extraction Methods and Tools'
solution = 'Platform'
+++

# Extraction Methods and Tools

The following diagram illustrates how the various extraction/replication
methods might fall and interact within a DSP
solution:

![](../../../Resources/Images/Extraction%20Methods/Extraction%20Methods%20Tools.png)

## SAP RFC & BOA RFC

RFC allows for the extraction of SAP pooled and clustered tables. The
RFC extraction method calls an RFC on the SAP application server to run
a SQL command. Data is returned in a Binary Large Object (BLOB) in
blocks (e.g., 10,000 records) that are then parsed by using SAP RFC, BOA
RFC or BODS RFC. The RFC is called again to extract the next block of
records (in this example, the next 10,000 records). The process repeats
until the entire table has been extracted.

## Assemble

Assemble is a tool within the DSP that creates and executes packages to
transfer data between systems. The tool uses an ODBC connection with a
non individual-specific account with read-only access. Once a connection
is established to a source, packages to refresh data are relatively easy
to create and process in the DSP.  Assemble runs multiple threads and is
the BackOffice Associates® preferred extraction method for all but the
largest tables.  Additional configuration and tuning can be required for
the largest tables that are over several million records (refer to the
[DSP Collect Delta Configuration](#DeltaConfiguration) image).

## SSIS (SQL Server Integration Services)

A component of MS SQL Server, SSIS replaces Data Transformation Services
(DTS). SSIS is typically faster than Assemble because a single program
is both reading the source and loading the target. Depending on
variables like hardware, connections and table width, SISS can achieve
extraction speeds of several million records per minute. However, using
SSIS to extract too many tables simultaneously can require additional
CPUs and memory on the application server. Consequently, SSIS should be
used judiciously to extract tables that cannot be efficiently extracted
with other methods. The same delta configuration that can be implemented
for Assemble can also be for SSIS when needed (refer to the [DSP Collect
Delta Configuration diagram](#DeltaConfiguration)).

## DBMoto®

DBMoto® functionality (which is housed in Collect) that uses an ODBC
connection to download data in any of three different ways: Refresh,
Change Data Capture (or Mirroring) and Synchronization.

In Refresh mode, an entire table is extracted. A one-time full-table
refresh is required for any tables that will be set up for change data
capture or synchronization. Change data capture mirrors data changes
made in a source system to a target system. Synchronization pushes data
changes both directions between two systems. 

When performing change data capture or synchronization, DBMoto®
leverages native change logs within the source to identify the subset of
records that have been changed and need to be updated in the target
system. If the source system does not contain native or accessible
change logs, then DBMoto uses triggers on the source system to push
changes.

## Choose the Right Extraction Method

To aid in selecting the right extraction methods for the project, refer
to the following table:

<table>
<tbody>
<tr class="odd">
<td><p>Connection Type</p></td>
<td><p>Extraction Method</p></td>
<td><p>Pros</p></td>
<td><p>Cons</p></td>
<td><p>Examples</p></td>
</tr>
<tr class="even">
<td><p>RFC</p></td>
<td><ul>
<li>BOA RFC</li>
<li>SAP RFC</li>
<li>BODS RFC</li>
</ul></td>
<td><ul>
<li>Ability to extract pooled tables, clustered tables and long text</li>
<li>Standard SAP protocol</li>
<li>Refresh can be scheduled within Collect</li>
</ul></td>
<td><ul>
<li>Slower than ODBC</li>
<li>Single thread to limit the number of jobs running at one time</li>
</ul></td>
<td><p>Material Long Text</p></td>
</tr>
<tr class="odd">
<td><p>ODBC</p></td>
<td><p>Assemble</p></td>
<td><ul>
<li>Multi-threaded for fast extraction of all but the largest tables (BOA preferred method)</li>
<li>Not tied to a specific version of SQL Database Management System (DBMS)</li>
<li>Supports fixed and delimited widths, and Excel.</li>
<li>Can configure batch size, select execution by field (e.g., change dates) and the number of parallel threads</li>
<li>Query can be optimized to be executed on source database</li>
<li>Very quick to initially build in the DSP</li>
<li>Refresh can be scheduled within Collect</li>
</ul></td>
<td><ul>
<li>For use only with transparent tables</li>
<li>Diminished performance when pulling very large record sets (&gt; several million)</li>
</ul></td>
<td><ul>
<li>Material Master</li>
<li>Customer</li>
<li>Product Hierarchy</li>
<li>Check &amp; Configuration tables</li>
</ul></td>
</tr>
<tr class="even">
<td><p> </p></td>
<td><p>SSIS</p></td>
<td><ul>
<li>Improved performance over Assemble for many system types. Can extract millions of records per minute, depending on hardware, software, table width, etc.</li>
<li>Filters can be applied to tables that maintain create and update dates in order to limit the data extracted. In this case, the logic and overhead to perform the delta on the full table copy is done in the DSP.</li>
<li>Refresh can be scheduled in Collect</li>
</ul></td>
<td><ul>
<li>For use only with transparent tables</li>
<li>Running many table extractions simultaneously with SSIS can require additional CPUs and memory</li>
<li>Requires additional configuration in DSP to set up as a delta update</li>
</ul></td>
<td><p>Largest master data or transactional tables where Assemble extraction is not sufficient. Historical examples include:</p>
<ul>
<li>Open Items</li>
<li>Bill History</li>
</ul></td>
</tr>
<tr class="odd">
<td><p> </p></td>
<td><p>DBMoto (Collect)</p></td>
<td><ul>
<li>Can extract data through Refresh, Change Data Capturing (mirroring) or Synchronization modes</li>
<li>Change data capture and synchronization leverage a source system’s native change logs or use triggers to identify the subset of data that has changed, thereby reducing the amount of data being extracted</li>
<li>Small footprint</li>
<li>Highly configurable through GUI</li>
</ul></td>
<td><p>If trigger-driven (no native change logs), changes to the source system are required (triggers and trigger tables for the tables that are going to be replicated with DBMoto)</p></td>
<td><p>Largest master data or transactional tables where Assemble extraction is not sufficient. Historical examples include:</p>
<ul>
<li>Open Items</li>
<li>Bill History</li>
</ul></td>
</tr>
</tbody>
</table>

## <span id="DeltaConfiguration"></span>Collect Delta Configuration

For large tables with requisite date fields, a delta extraction process
can be built in within DSP, as conceptualized in the following
diagram:

![](../../../Resources/Images/Extraction%20Methods/For%20large%20tables%20with%20requisite.png)
