+++
title = 'Enable Audit Trail and Electronic Signature'
solution = 'Platform'
+++

# Enable Audit Trail and Electronic Signature

Any edits to a record can be tracked through an Audit Trail. When the
Audit Trail is enabled on a table, an **Audit** icon displays next to
each record. Clicking the icon opens a window that displays the date and
time of the change, who changed the record, and the values before and
after the change.

When Audit Trail is enabled, three tables are automatically created in
the database: **XXXXAudit**, **XXXXAuditColumn** and
**XXXXAuditProcedure**, where **XXXX** is the name of the table being
audited. It is important to decide if the Audit tables are to reside in
the same database as the application tables or in a different database.
If using a separate database, register the database in the System
Administration WebApp as a data source.

An electronic signature is a digital signature of a token representing
the changes and is used in conjunction with the Audit Trail feature
enabled. The token is computed by concatenating the user ID and the
process token. The string is hashed using the MD4 algorithm. The
resultant binary value is the signature. The value is stored in the
**\#Audit** table using Base 64 encoding.

This method provides a fast and simple digital signature implementation.
It is important to note that the authenticity of an electronic signature
depends on restricting access to the audit tables. If an unauthorized
user gains write access to the audit tables, the signature can be forged
or the audit trail could be altered.

This section contains these topics:

  - [Enable Audit Trail on a Page](Enable_Audit_Trail_on_a_Page.htm)
  - [Enable Electronic Signature](Enable_Electronic_Signature.htm)
  - [Drop Audit Trail](Drop_Audit_Tables.htm)
