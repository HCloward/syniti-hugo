# Security Definition Example

As an example, to create a role that gave access to a technical analyst
with access to the dgSAP target that can post Integrate processes
defined in the Materials category, the following could be done:

1.  Create a Role named “Technical Analyst”
2.  Assign the following keys:
      - Collect Targets – dgSAP
      - Analyze DataSources – dgSAP
      - Integrate Categories – Materials
3.  Assign the following WebApp groups:
      - Collect – PowerUser
      - Analyze – User
      - Integrate – PowerUser

Any and all users that need the access of a Technical Analyst would then
be assigned to the role, thereby giving them access to the necessary
components and data within.
