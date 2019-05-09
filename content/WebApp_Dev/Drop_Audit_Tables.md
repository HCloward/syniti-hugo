+++
title = 'Drop Audit Tables'
solution = 'Platform'
+++

# Drop Audit Tables

Two users are required to drop audit tables.The first user requests the
drop and within 24 hours, the second user drops the audit tables.

Refer to [Enable Audit Trail & Electronic
Signature](Enable_Audit_Trail_Electronic_Signature) for general
information.

To drop the Audit Trail:

1.  Click **Admin** \> **Data Sources** on the *Navigation* pane.

2.  Click **Audit** for the WebApp’s data source.

3.  Click **Tables** 

4.  Click **Vertical View**.

The first user clicks the **Request Drop** button. A message displays,
confirming a request has been submitted. Both the **RequestDrop** and
the **Drop Audit Tables** buttons are inactive.

If the second user does not click the **Drop Audit Tables** button
within 24 hours, the button becomes inactive and the process needs to be
initiated again. Once the button is clicked, the audit is dropped. When
Audit is dropped, the audit tables remain in the database. Once the
Audit is dropped, the record must be deleted on the *Audit Tables* page.

**NOTE:**   Dropping an Audit table is
**<span class="underline"><span style="color: #ff0000;">not</span></span>**
workflow enabled; verbal communication between the two users involved is
required.
