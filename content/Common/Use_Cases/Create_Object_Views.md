+++
title = 'Create Object Views'
solution = 'Platform'
+++

# Create Object Views

The first step in setting up duplicate detection is to create a view
that checks the object for duplicate records.

Create a view in the Common database that references an object (vendor,
customer, material, etc.), a key and all relevant columns for Duplicate
Detection. The view must include a single key field (use concatenation
if more than one field to create the key exists in the table). Up to
five columns can be used for duplicate comparison.
