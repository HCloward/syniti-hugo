# Set the Y-axis of a Chart with the Value Column Property

Value column properties are used to specify which field within the
web\*Chart view corresponds to a Y-axis value. This column is expected
to be a numeric type because charts can only display numeric ranges.
Multiple Value columns are supported when there is only one Category
column defined. When the graph renders, there will be *n* number of
series. For example, if a web\*Chart view renders \[“1/1/1990”, 1, 2,
3\], the first column would be defined as the Category column and the
last three columns would be defined as Value columns. Value columns are
recommended over a Secondary column when the amount of supplemental data
is static.
