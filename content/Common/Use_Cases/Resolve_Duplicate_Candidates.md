# Resolve Duplicate Candidates

Once duplicate records are identified, which are referred to as
*unresolved candidates* at this point, they must be manually reviewed to
determine what is an actual duplicate record and what is a unique
record.

To resolve duplicate candidates:

1.  Click **Analyze** in the *Navigation* pane.

2.  Click **Duplicates** for Data Source ID.

3.  Click **Unresolved Candidates** for Object.
    
    [View the field descriptions for the Candidates
    page](../Page_Desc/Candidates.htm)

4.  Decide if a duplicate pair should use the original value, use the
    duplicate value or is a non duplicate.

5.  Options for resolving duplicate candidates are:
    
      - **Merge Left** – Click to keep the original value and discard
        the duplicate value.
      - **Not Duplicate** – Click if the value is not a duplicate, but
        rather a unique value.
      - **Merge Right** – Click to use the duplicate value and discard
        the original value.
    
    **NOTE:** Use caution when deciding what is a duplicate record. A
    duplicate source record can be used over another source record. A
    duplicate ERP record can be used over a duplicate source record. But
    do not use a duplicate source record over an ERP record – this can
    be accommodated by adding a NoChange column to the duplicate
    detection view and setting the value to 1.

The following example illustrates the results of NoChange = 1 on the SAP
account. It is not possible to merge the SAP record into the Oracle
record.

CREATE VIEW dDup.dbo.tvDEMO\_NoChange\_FLAGSel as

   SELECT ObjectID, Name, Street, City, Region, PostalCode, Phone,
zSource,

          (select 1 where zSource = ‘SAP’) as NoChange

     FROM AddressServer.dbo.ttADRC

    WHERE ObjectType = ‘Vendor’
