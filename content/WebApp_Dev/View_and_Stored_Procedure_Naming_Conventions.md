+++
title = 'View and Stored Procedure Naming Conventions'
solution = 'Platform'
+++

# View and Stored Procedure Naming Conventions

Naming conventions are essential as they make development easier, and a
standardized set of naming conventions allows other application
developers to understand behaviors and configuration.

Views have different sets of naming conventions. The default naming
conventions display on the *WebApps* page’s *Vertical* View on the
Naming Conventions tab. When naming views, follow these conventions.

By default, view names start with web\* which allows a developer
reviewing/debugging SQL to differentiate between table/view queries.
Views must also include the relevant table name after the “web” to
denote which base record set the view operates against if the target
WebApp has the Enforce Strict Naming option enabled. The view may also
contain a brief (one or two word) description of the view’s selection
criteria. For instance, if a customer is “Inactive,” the view may start
with “webCustomer\_Inactive.” Refer to [Naming Conventions and the
Enforce Strict Naming
Feature](Naming_Conventions_and_the_Enforce_Strict_Naming_Feature)
for more information.

Lastly, view names are suffixed with an operation abbreviation for their
associated usage. For application development, a list of these can be
found on the *Vertical* View of the *WebApps* page (Admin \> WebApps \>
Vertical View \> Naming Conventions tab). Other non-enforced naming
conventions that are commonly used are “Sel” (to indicate it is
**sel**ecting a subset of data) and “Count” (to indicate it is selecting
some aggregate or metric data based on the primary table). Underscores
can be used to increase readability of the view name.  For example, the
full named view “webCustomer\_NameStartsWithLetterASel” returns a record
set of all customers with names starting with “A.”

Procedures have similar naming conventions, but suffix with Upd (for
update), Del (for delete), and Ins (for insert logic).
