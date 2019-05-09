+++
title = 'Incorporate the Security View into Request Processing'
solution = 'Data Quality'
+++

# Incorporate the Security View into Request Processing

This section provides an example of implementation of Org Units.

**NOTE**: Org Units should only be used by advanced users, such as
BackOffice Consultants, who are familiar with DSP® Development.

**NOTE**: If the data entry table does not exist when the template is
generated, the security view will not be automatically generated. This
situation can occur when the template is a custom template with custom
data entry pages.

**NOTE**: If the value entered in **TEMPLATE COLUMN** on the *Template
(Org Units)* page does not exactly match a column in the data entry
table, that Org Unit will be excluded from the generated security view.
To add the Org Unit, the security view will have to be manually modified
to include a join from the TemplateColumn name in the Org Unit table to
the appropriate column in the data entry table.

Once a request with Org Units has been saved, there is no automatic
connection between the Org Unit security and request data on the Data
Entry pages. This connection must be made manually behind the scenes by
a Template Administrator
<span style="font-family: Arial, sans-serif;">as described in this
section.</span>

A Template Administrator must modify the horizontal view for Data Entry
page(s) so that only users with security for the record (as in, only
users who are assigned to the Org Unit Values that are used on the
request) can see the record on the Data Entry page.

<span style="font-weight: bold;">NOTE</span>: For requests with Org
Units that use a mass change, if the
<span style="font-style: italic;">Horizontal</span> View of the Data
Entry page has been modified to include the security view and boaUserID,
only the records to which the user has access will be updated when mass
change is executed.

The horizontal view contains only the Data Entry table. Add the security
view and join on RequestID and ID, as in the example below. Select
boaUserID for output.

 

![](../../../Resources/Images/image012.jpg)

Security can be further customized so that users can only edit and
delete records for which they have security; others will be visible but
will not allow updates.

To further customize security:

1.  The delivered DCV views do not include boaUserID, so both
    ttUserTemplateRole and the security view must be added
    <span style="font-family: Arial, sans-serif;">to the delivered
    DCV</span>. Note the outer joins in the example below.
2.  Select ttUserTemplateRole.UserID and alias as "boaUserID."
3.  Modify delivered boaEdit logic to take into account the security
    view. See the example below.
4.  Add boaDelete logic. See the example below.

![](../../../Resources/Images/image014.jpg)

 

To modify boalogic as mentioned in step 3 above"

 

ISNULL((SELECT 0 AS Expr1 WHERE (dbo.ttChangeMaterial.LockReject = 1)
AND (cMass.dbo.ttTemplateRole.RoleType = 'Review')), 1) \*
ISNULL((SELECT 0 AS Expr1 WHERE
(dbo.webChangeMaterial1SecuritySel.boaUserID IS NULL)), 1) as boaEdit

 

To add boalogic delete logic as mentioned in step 4 above

<span style="font-size: 11.0pt;">:</span>

<span style="font-size: 11.0pt;">ISNULL((SELECT 0 AS Expr1 WHERE
(dbo.webChangeMaterial1SecuritySel.boaUserID IS NULL)), 1) as
boaDelete</span>

Once these changes have been made, subsequent requests submitted for the
template will follow the security settings configured here.

Refer to [Updates to Finishing a Data Role for Templates with the
Security View](Updates_to_Finishing_a_Data_Role_for_Templates) and
[Add the Org Unit Security View to Template Role Validation
Rules](Add_the_Org_Unit_Security_View_to) for more information.
