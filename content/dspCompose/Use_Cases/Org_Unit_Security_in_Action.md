# Org Unit Security in Action

Once the security view has been incorporated into request processing,
Org Units can be used to restrict data on the Data Entry page and
restrict which updates are performed in a mass change. Additionally,
once the security view has been added to a Template Role validation rule
(if the template uses validation rules), template role validation
failures will be limited to records associated with the current user’s
Org Unit values.

To understand how the security could work, consider this example.

A Template has the Org Units Plant and SalesOrg assigned.

Users have been assigned to the following Org Unit values for the
template:

  - JSmith is assigned Plant A, SalesOrg 1, SalesOrg 2
  - HMartin is assigned Plant A, SalesOrg 2
  - RJones is assigned Plant A, SalesOrg 3

A user creates a request based on the template. The request is assigned
the following Org Units and Org Unit values.

  - Plant A
  - SalesOrgs 1 & 2

Data records for the request are:

  - ID 1, Plant A, SalesOrg 1
  - ID 2, Plant A, SalesOrg 1
  - ID 3, Plant A, SalesOrg 2

After configuring security manually using the security view and updating
the template role validation rule:

  - JSmith has security for record IDs 1, 2 & 3 and will see validation
    failures related to records from these Org Unit values. If JSmith
    performs a mass change, only records from these values will be
    updated.
  - HMartin has security for record ID 3 and will only see validation
    failures related to records from this Org Unit value. If HMartin
    performs a mass change, only records from this value will be
    updated.
  - RJones does not have security for any of the data records
