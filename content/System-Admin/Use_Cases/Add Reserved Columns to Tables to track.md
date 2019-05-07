+++
title = 'Add Reserved Columns to Tables to Track Excel Integration'
solution = 'Platform'
+++

# Add Reserved Columns to Tables to Track Excel Integration

To track the user and date/time of data entry during the Excel import
process, the Page Designer must add the reserved columns to any tables
related to the pages used by Excel Integration. The values will be
updated upon completion of the import process.

Refer to [Add Reserved Columns to
Tables](../../WebApp_Dev/Add%20Reserved%20Columns%20%20to%20Tables.htm)
for more
information.

|              |                                                                                                                                             |
| ------------ | ------------------------------------------------------------------------------------------------------------------------------------------- |
| System Field | Description                                                                                                                                 |
| AddedOn      | Contains the date/time that the record was inserted into the table.                                                                         |
| AddedBy      | Contains the username of the user that imported the record.                                                                                 |
| AddedVia     | Contains the method used to add the record into the table. This field defaults to ‘ExcelImport’ for records inserted via Excel Integration. |
| LockedOn     | Contains the date and time the record was locked.                                                                                           |
| LockedBy     | Contains the name of the user who has the record locked.                                                                                    |
| boaLockType  | Contains the method, in this case “Locked via Excel Integration.”                                                                           |
