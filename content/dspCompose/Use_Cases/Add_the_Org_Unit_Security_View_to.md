# Add the Org Unit Security View to Template Role Validation Rules

Role validations allow for template-specific data standards to be
applied at both the role and the request level. dspCompose™ runs
validations registered for roles when a user assigned to that role
enters a record for the request, or when a user clicks Validate for a
role on the *Request (Roles)* page.

**NOTE**: Role validations are views stored in a data source, typically
the cMass\_Data database. The view must exist before the role validation
can be added to the template.

Adding the Org Unit security view to template role validation rules is
not required for Org Units to work, but is required if a template uses
template role validation rules.

A Template Administrator must add the security view to a Template Role
validation rule so that Org Unit security can then restrict validation
failures to records associated with Org Unit Values, and users will only
see validation failures for records they can access.<span> </span>

For example, a template with Org Units assigned has two users with two
different Org Unit Values assigned. User A is assigned to Plant A. User
B is assigned to Plant B.

A Template Administrator adds a Template Role validation rule to the
template and adds the Org Unit security view to that validation rule.

If a record with data from Org Unit value Plant A fails the validation
rule, User A will see the validation failure and User B will not.

If the Template Administrator had not added the security view to the
Template Role validation view, User A and User B would both have seen
the failure, even though User B did not have access to the record that
caused the failure.
