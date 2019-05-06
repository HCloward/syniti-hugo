# How the DSP Uses Data Source Types

<table>
<tbody>
<tr class="odd">
<td><p>Data Source Type</p></td>
<td><p>Use in DSP</p></td>
</tr>
<tr class="even">
<td><p>Data Services Repository</p></td>
<td><p>Used by dspMigrate and Collect to execute batch jobs via SAP's Data Services application. Used also by Integrate to execute batch jobs for loading purposes.</p></td>
</tr>
<tr class="odd">
<td><p>SAP Application Server</p></td>
<td><p>Used by:</p>
<ul>
<li><p>Collect to populate 'sdb' and 'dg' databases via RFC.</p></li>
<li><p>Integrate to post data to SAP's ERP application.</p></li>
</ul></td>
</tr>
<tr class="even">
<td><p>IGUC</p></td>
<td><p>Used by:</p>
<ul>
<li><p>Collect to populate 'sdb' and 'dg' databases from any application Boomi can connect to.</p></li>
<li><p>Integrate to post data to any application Boomi can connect to.</p></li>
<li><p>Any custom DSP WebApp.</p></li>
</ul></td>
</tr>
<tr class="odd">
<td><p>ODBC</p></td>
<td><p>Used by Collect or Assemble to populate 'sdb' and 'dg' databases.</p></td>
</tr>
<tr class="even">
<td><p>OleDB</p></td>
<td><p>Used by Collect or Assemble to populate 'sdb' and 'dg' databases.</p></td>
</tr>
<tr class="odd">
<td><p>Oracle</p></td>
<td><p>Used by Collect or Assemble to populate 'sdb' and 'dg' databases.</p></td>
</tr>
<tr class="even">
<td><p>Migration Source Database</p></td>
<td><p>Used heavily by dspMigrate. Populated by Collect or Assemble.</p></td>
</tr>
<tr class="odd">
<td><p>Migration Object Database</p></td>
<td><p>Used heavily by dspMigrate, especially Transform. Commonly used by Integrate and dspMonitor.</p></td>
</tr>
<tr class="even">
<td><p>Target System Database</p></td>
<td><p>Used heavily by dspMigrate, dspCompose, and dspConduct. Populated by Collect or Assemble.</p></td>
</tr>
<tr class="odd">
<td><p>Local Utility Database</p></td>
<td><p>Typically used to hold SQL objects for the development/operation of a custom DSP Webapp.</p></td>
</tr>
<tr class="even">
<td><p>Local File</p></td>
<td><p>Used by:</p>
<ul>
<li>Collect, Common, dspConduct, dspMonitor, Integrate, Map, and Transform to write files to the DSP application server.</li>
<li>Assemble to read from or write to a file.</li>
</ul></td>
</tr>
<tr class="odd">
<td><p>Remote File (HTTP)</p></td>
<td><p>Used by Assemble to read from or write to a file.</p></td>
</tr>
<tr class="even">
<td><p>Remote File (FTP)</p></td>
<td><p>Used by Assemble to read from or write to a file.</p></td>
</tr>
<tr class="odd">
<td><p>Remote File (UNC)</p></td>
<td><p>Used by Assemble to read from or write to a file.</p></td>
</tr>
</tbody>
</table>
