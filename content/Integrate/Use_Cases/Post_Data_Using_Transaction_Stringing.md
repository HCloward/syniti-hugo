+++
title = 'Post Data Using Transaction Stringing'
solution = 'Platform'
+++

# Post Data Using Transaction Stringing

A process with multiple templates that uses the synchronous post
execution method can use a Return Value, a value returned from the
target system, from a template registered to the process when posting
subsequent templates in the process.  A template with a high priority
can use a Return Value from a template with a lower priority in
posting.  This process is called Transaction Stringing. 

Transaction Stringing can use process information from one template
(transaction) in a second template (transaction), or it can process two
similar transactions within one upload.

For example, transaction stringing can be used to process a template
creating a material (MM01) in SAP, then process a second template
creating a corresponding information record (ME11). Because the material
number is not known at the time the second data source is created, the
material number can be passed in from the first data source after the
first data source has processed. 

**NOTE**: Only multiple template processes based on a BDC Script, GUI
Script or BAPI/RFC template types can use transaction stringing. The
process must use the synchronous post execution method. Refer to [Create
a Process](Create_a_Process) for more information.

**NOTE**: Transaction Stringing cannot be configured if the process is
active.

<span style="font-weight: bold;">NOTE</span>: After Post Rules can be
added to run after a template in a multi-template process. These rules
return data that is used as an input parameter for the next template in
the process. Refer to [Register After Post Rules to a Process
Template](Register_After_Post_Rules_to_a_Process_Template_Overview)
for more information.

To configure Transaction Stringing:

1.  Create multiple templates based on the data that will be passed from
    one transaction to another.
    
    **NOTE**: These templates must be of the type GUI Script, BDC Script
    or BAPI/RFC. Refer to
    [*<span style="color: #0000ff;font-style: normal;">Record a BDC
    Script</span>*](Record_a_BDC_Script),
    [*<span style="color: #0000ff;font-style: normal;">Record a GUI
    Script</span>*](Record_a_GUI_Script), or
    [*<span style="color: #0000ff;font-style: normal;">Configure a BAPI
    Template</span>*](Configure_a_BAPI_Template) for more
    information.

2.  Activate the templates.

3.  Create a process that includes the template that will generate the
    Return Value used during transaction stringing and uses the
    Synchronous Post Execution Method. Refer to [Create a
    Process](Create_a_Process) for more information.

4.  Add the remaining templates to the process. Refer to
    *<span style="color: #0000ff;font-style: normal;">[Add Templates to
    a Process](Add_Templates_to_a_Process)</span>* for more
    information.
    
    **NOTE**: Set the priority order of the templates in the order they
    should be processed using transaction stringing.  Templates are
    processed in ascending priority order. A template with a low
    priority is processed before a template with a high priority.

5.  Configure the process template loop field mappings to set the return
    value template and the value to be passed using transaction
    stringing.

To configure the process template loops and field mappings to use return
values on the *Process* page:

1.  Click the **Templates** icon for a process.

2.  Click the **Loops** icon for the parent template in the process.
    
    **NOTE**: The **INCLUDE** check box should not be used for process
    template loops for a process that posts using the Synchronous Post
    Execution Method. When posting, the user must post the entire
    template.

3.  Click **Edit**.

4.  Enter **PKey** in **PRIMARY KEY COLUMN NAME**.

5.  Click **Save**.

6.  Click **Field Mappings**.
    
    **NOTE**: The **TEMPLATE FIELD UNIQUE NAME** and the **DESCRIPTION**
    field should have data for all records.

7.  Click **Edit**.

8.  Enter either a **MAPPINGVALUE** or a **FIXEDVALUE** for every field.

9.  Click **Save**.

10. Navigate to the *ProcessTemplate* page.

11. Click **Loops** for the child template that will use the value
    passed from the parent template.

12. Click **Edit**.

13. Select the view that will provide the data for the child template’s
    field mappings in the **VIEW NAME** list box. 

14. Enter **PKey** in **PRIMARYKEYCOLUMNNAME**.

15. Click **Save**.

16. Click **Field Mappings**.
    
    **NOTE**: The **TEMPLATE FIELD UNIQUE NAME** and the **DESCRIPTION**
    field should have data for all records.

17. Click **Edit**.

18. Enter either a **MAPPING VALUE** or a **FIXED VALUE** for every
    field except the field that will use the Return Value. This field
    should not have data in either **MAPPING VALUE** or **FIXED VALUE**.

19. Click **Save**.

20. Click *Vertical* View for the field that will use the Return Value.

21. Click **Edit**.

22. Select the parent template that will pass the return value to the
    current template in the **Return Value Template ID** list box.

23. Select an option from the **Return Value** list box.
    
    **NOTE**: The Return Value contains the data to pass to the current
    field. SAP returns up to four return values for each posting and the
    return values differ for each transaction code.  The return values
    make up the dynamic part of the message that displays to the user in
    SAP in the status bar after saving the record. For example:  
    
    MM01:  Message displayed “Material **101** created successfully”.
    
                                  Return Value 1: 101 = Material Number
    
     
    
    FB50: Message displayed “Document **123235** was posted in company
    code **0001**”
    
                                  Return Value 1: 123235 = Document
    Number
    
                                  Return Value 2: 0001 = Company Code

To determine the Return Values to select in the **Return Value** list
box, execute the transaction used by the template manually in SAP and
monitor the status bar to determine which return values are passed back
via SAP.

24. Click **Save** once the Return Value template and Return Value are
    set.
    
    **NOTE**: On the *Horizontal* View of the *Process Template Loop
    Field Mappings* page, the **RV** column displays a check mark for
    the field that will use the Return Value.

25. After the field mappings have been configured, post the process
    using the **StandardSAPPostingBDC Post Method**.

26. Set up testing scenarios, if necessary, for a process with multiple
    templates on the **Advanced** tab on the *Process Post Vertical*
    View to restrict the number of templates that Integrate posts. Enter
    the priority of the first template to include in the debug process
    in the **Start Template Priority** field, and the priority of the
    last template in the **End Template Priority** field.

27. Post the data. If the posting fails, troubleshoot the errors using
    information on the *Messages* page or download the message file on
    the *Message File* page. Refer to [Posting
    Troubleshooting](Posting_Troubleshooting) for more information.

28. Resubmit the post after correcting any errors. Click **Reset** for
    the process post on the *Process Post* page’s *Vertical* View on the
    **Posting** tab, then post the data again.
    
    **NOTE**: After resetting a post it can be submitted again
    regardless of its status prior to the reset, and regardless of the
    reason for the failure.
