+++
title = 'Enable Auditing for Tables with Personal Information'
solution = 'Platform'
+++

# Enable Auditing for Tables with Personal Information

On a client’s site, a System Administrator must enable auditing for any
tables that contain personal data or that must be purged for compliance
reasons.

At the client site, an Administrator must also set up auditing for these
specific tables in the DataSource named “Data Garage'.

  - dgTarget
  - dgTargetSource
  - dgTargetSourceTable

When a Data Controller updates any retention expiration date, an
e-signature is required and captured in the audit records.

At the target, target source or table level, a Data Controller can
update the retention expiration date, which sets when data is purged at
that level. If this date is updated, it is audited and an e-signature is
required.

To set up auditing, use the DSP’s auditing feature. Refer to [Enable
Audit Trail and Electronic
Signature](../../WebApp_Dev/Enable_Audit_Trail_Electronic_Signature.htm)
for more information.
