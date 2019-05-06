# Partition Logic Semantically

An application’s value is not measured in SQL object count. Centralizing
logic can help consolidate an application into smaller, more manageable
chunks.

For example, several “Customer” based pages select records from the
Customer table. The table has an “Active” bit, and can be modified so
that only “Active” customers show up on these pages. Many of these
existing “webCustomer\*Hor” views may already have complex WHERE
clauses. Appending “\[Active\] = 1” to every WHERE clause adds
complexity to the WHERE clause, and makes it less readable and
cumbersome to maintain. Instead, create a supplemental active view such
as “webCustomer\_ActiveSel” and replace all of the “FROM \[Customer\]”
sections with FROM \[webCustomer\_ActiveSel\]. This way, if the
definition of “Active” changes, it’s an easy change in one view, instead
of many.

Procedures are another common place to consolidate logic. SQL stored
procedures can be considered object oriented code in the eyes of the
developer. Consolidate any logic that is more complex than a single SQL
statement into a procedure. This greatly reduces the chance of bugs
occurring, and centralizes the logic so that a developer doesn’t have to
remember where everything is.

For example, place logic such as “When I see an update to set a field to
1, I also now need to go set this other field to 2” into a stored
procedure. Updates to this logic can then be added in a single place.
