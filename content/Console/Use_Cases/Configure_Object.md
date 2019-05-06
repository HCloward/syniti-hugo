# Configure an Object

A migration object is assigned to a Wave-Process Area
combination.  Examples of objects include customers, basic materials,
price lists or sales orders.

To configure an object:

  - [Add Contacts for an Object](#Add)
  - [Add Decisions for an Object](#Add2)
  - [Copy or Move an Object](Copy_Elements.htm#Copy3)
  - [Track Object History](#Track)

## <span id="Add"></span>Add Contacts for an Object

Contact information can be associated with an Object to send workflow
emails to contacts during object creation and when working with
decisions. Users, whether registered in the platform or not, can be
notified via email of any Object design changes.

**NOTE**: Contacts may or may not be platform users or members of the
Project Team.  Often they are subject matter experts in the Business
Units.

<span style="font-weight: bold;">NOTE</span>: Contacts can be added for
targets in Target Design. Refer to [Add Individual Target
Contacts](Add_Target_Contacts_to_Objects.htm#Add2) for more information.

To add a contact in Console:

1.  Navigate to the *Objects* page.

2.  Click the**Contacts** icon for the object.

3.  Click **Add**.
    
    *[View the field descriptions for the Object Contacts
    page](../Page_Desc/Object_Contacts.htm)*
    
    **NOTE:**The CONTACT list box displays all users registered in the
    platform. Users who are not registered in the platform can be added
    by clicking the + sign at the top of the list box.

4.  Select a user name from the **CONTACT** list box.  
    Or  
    Enter a name in the list box and press **Enter**.

5.  Select a job function from the **POSITION** list box.
    
    **NOTE:** Refer to [Configure List Box
    Values](Configure_List_Box_Values.htm) for information on how to
    modify **Position** options.

6.  Enter a telephone number in the **PHONE** field.

7.  Enter a valid email address in the **EMAIL** field.

8.  Enter an address/office in the **LOCATION** field.

9.  Select an option in the **TIME ZONE** list box.

10. Enter additional comments about the contact in the **COMMENT**
    field.

11. Click the **SEND WORKFLOW** check box to indicate the contact should
    be notified when an Object design change occurs or when a decision
    is modified. Refer to Add Decisions for an Object for more
    information.

12. Click **Save**.

## <span id="Add2"></span>Add Decisions for an Object

A decision allows a group of users to communicate about migration
project questions using Console, and to consult a single source to track
questions as they are discussed and resolved.

Decisions can also document project standards, such as naming
conventions.

Before adding a decision, contacts must exist for the Object. The **SEND
WORKFLOW** check box must be checked for the contact to receive
notifications about decisions.

Refer to [Add Contacts for an Object](#Add) for more information.

To add a decision in Console:

1.  Navigate to the *[Objects](../Page_Desc/Objects_H.htm)* page.
    
    **NOTE**: Access the page by:  
    Selecting **Elements \> Object** on the *Navigation* pane.  
    Or  
    Clicking **Objects** on the *[Wave: Process
    Areas](../Page_Desc/Wave_Process_Areas.htm)* page, and clicking an
    object in the **OBJECT ID** column.

2.  Click **Decisions** for an Object.

3.  Click **Add** in the *Objects Decisions* page in the child pane.
    
    *[View the field descriptions for the Object Decisions
    page](../Page_Desc/Object_Decisions_H.htm)*

4.  Select a decision type from the **TYPE** list box.
    
    **NOTE:** Refer to [Configure List Box
    Values](Configure_List_Box_Values.htm) for information on how to
    modify Type options.

5.  Enter a discussion topic in the **TOPIC** field.

6.  Enter a decision that requires an action in the **DECISION** field.

7.  Select a decision status from the **STATUS** list box.

8.  Click the **WORKFLOW** check box to enable it to send emails about
    the decision to the object’s contacts.

9.  Select a value from the **APPLICATION** list box to identify the
    application for which the decision is being made.

10. Enter the name of the field affected by the decision in the **FIELD
    NAME** field.

11. Enter the next action required for the decision in the **NEXT
    ACTION** field.

12. Enter a date or click the Calendar to select a date in the **NEXT
    ACTION DUE BY** field.

13. Click **Save**.

14. Click the **Comments** icon; the *Object Decision Comments* page
    displays.
    
    *[View the field descriptions for the Object Decision Comments
    page](../Page_Desc/Object_Decision_Comments.htm)*
    
    **NOTE**: If no records exist, the page displays in add mode.
    Otherwise, click **Add** .

15. Enter a question about the decision in the **COMMENT** field.

16. Click **Save**.

**NOTE**: Console sends an email to the contacts associated with the
object. 

## <span id="Track"></span>Track Object History

A migration Object is assigned to a Wave-Process Area
combination.  Examples of Objects include customers, basic materials,
price lists or sales orders.

The history for an Object displays on the *[Object
History](../Page_Desc/Object_History_H.htm)* page.

An Object's history is not tracked by default. Tracking must be enabled
before the Object's history is recorded.

To configure Console to track history:

1.  Select **Elements \> Object** from the *Navigation* pane.

2.  Click the **Vertical View** icon for an Object.

3.  Click **Edit**.
    
    [View the field descriptions for the Object page’s Vertical
    View](../Page_Desc/Objects_H.htm)

4.  Check the **Build History** check box.

5.  Click **Save**.
