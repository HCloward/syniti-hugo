# When to use Value Columns Instead of a Secondary Column

It may seem intuitive to always use a Secondary category when each
record represents a separate value because Secondary categories give the
best angle to manipulate data. However, Secondary categories do not
allow for column properties that the Value columns support, such as
coloring individual lines or bars.

An example of when to use multiple Value columns instead of a Secondary
column would be for data within a finite number of possible states. For
instance, if there is a record that denotes Pass or Fail, there are only
ever going to be two individual series (the Pass series and the Fail
series). If a view is created to return the following data, “Green” can
be the color for Pass and “Red” for Fail. This kind of manipulation can
only be performed at the Value column level.
