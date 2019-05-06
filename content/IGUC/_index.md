+++
title = "IG Universal Connect Overview"
weight = 3
layout = "single"
solution = "Platform"
+++

# IG Universal Connect Overview

**NOTE:** Access to IG Universal Connect is by subscription. Contact
your BOA Sales contact for more information. If you do not have contact
information then post your question in the [Data Insiders
Community](../../Data%20Insiders%20Community.htm).

IG Universal Connect uses the DSP® combined with Dell Boomi, an
Integration Platform as a Service (IPaaS) solution. Boomi’s connectors
allow the DSP® to extract and load data in systems that do not use a
database connection, such as Workday, Salesforce or SAP SuccessFactors.

In Boomi, a DSP® Implementer creates Processes using the IG Universal
Connect Template. For information about the IG Universal Connect
Template, access the help center at <http://support.boaweb.com/hc/en-us>
and search for the article "[Configuring and Using the IG Universal
Connect
Template](https://support.boaweb.com/hc/en-us/articles/115011370988-Configuring-and-Using-the-IG-Universal-Connect-Template)."
The Boomi Process also has an associated atom, the default execution
environment (for example, Dev, QA and Prod).

**NOTE**: Boomi Processes are created on-site by the implementers
depending on requirements, business rules and other factors.

After the Process is created, it is registered in the DSP® in Common,
Collect or Integrate.

**NOTE**: When Integrate executes a Boomi process, it passes in the
LinkID for the execution, which is used to return a status to the DSP®
once the execution is complete. **The user must add any additional
parameters required for the process.**

IG Universal Connect can be used in many scenarios.

Migration between systems is no longer limited by database connections,
and data can be moved in and out of a wide variety of sources and
targets. Additionally, dspMigrate™ functionality does not change with
the use of IG Universal Connect.

For example, in an on–premise to cloud migration, a DSP® Implementer
could use Assemble to extract data from a legacy system into a source
database. After registering the IG Universal Connect data source in
Common, the DSP® Implementer uses an IG Universal Connect connection in
Collect to move the Target data and Target metadata to a Target
database. After completing the dspMigrate™ execution, an Integrate
Process Template based on an IG Universal Connect Template loads the
data into the cloud system.

In terms of data quality, using IG Universal Connect, data from a
cloud-based system can be extracted to a Target database in the DSP®. In
dspMonitor™, data errors can be identified, then corrected in
dspCompose™. The data can then be validated and loaded back into the
system using IG Universal Connect via Integrate.

Additionally, using a public plugin attached to an event on a custom
page, a WebApp Developer can execute cloud-based Processes created in
Boomi, such as making a web service call and displaying the results on a
custom page.

IG Universal Connect can also provision and host a web service on the
DSP® Application server that can expose any DSP® functionality that is
in a view, table or stored procedure in the SQL database. Refer to
"Configuring and Using the IG Universal Connect Template" on the BOA
support site for more information.

To use IG Universal Connect and the DSP® in any scenario:

• [Register the IG UC Data Source in
Common](../Common/Use_Cases/Register_a_Data_Source_in_Common.htm)

• [Extract Data Using IG Universal Connect in
Collect](Extract%20Data%20using%20IG%20Universal%20Connect%20in%20Collect.htm)

• [Post Data Using IG Universal Connect in
Integrate](Post%20Data%20Using%20IG%20Universal%20Connect%20Overview.htm)

In System Administration, refer to [Execute a Boomi Process from a
Custom
Page](../WebApp_Dev/Execute%20a%20Boomi%20Process%20From%20a%20Custom%20Page.htm)
for additional information.
