+++
title = 'Creating a Security View Guidelines'
solution = 'Platform'
+++

# Creating a Security View Guidelines

In most cases, Security Definition views should be created using the
original source of the data that the view will be securing against. This
way, when new records are added, the security view will implicitly
contain those records.

It’s also a good idea to apply the security definition to the page(s)
that maintain the source of the data. This way, the “Update User
Definition on Save” option can be enabled on those pages, ensuring that
the user who creates the data will always have implicit access.

Refer to [Set Security for a Custom
WebApp](Set_Security_for_a_WebApp.htm) for general information.
