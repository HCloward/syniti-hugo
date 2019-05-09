+++
title = 'Copy a Process'
solution = 'Platform'
+++

# Copy a Process

Use an existing process as the basis for a new process.

When Integrate copies a process, it copies:

  - All of the templates registrations assigned to the process

**NOTE**: If a process is copied to another category, the templates will
be copied but the template names will display as a GUID.

  - All of the template process loops for single or multiple loop
    templates, including the View Name and the Primary Key Column Name,
    the Flat File Object Key, the Download Tables and others
  - The field mappings for all process template loops
  - The Return Value Template ID and the Return Values, if the process
    uses transaction stringing
  - RFC parameters, if applicable
  - Relationships, if applicable
  - Allowed connections, if applicable

Integrate does not copy the process post records for the original
process. Integrate creates one process post by default for the copied
process.

**NOTE**: A process can be copied whether the process is active or not.

To copy a process:

1.  Select **Categories** on *Navigation pane*.

2.  Click the **Processes** icon for a category.

3.  Click **Vertical View** for the process that should be copied.

4.  Click the **Copy** tab.

5.  Click <span style="font-weight: bold;">Copy Process</span>.
    
    **NOTE**: The **Copy Type** field displays **Process**.

6.  Click **Edit**.
    
    *[View the field descriptions for the Copy
    page.](../Page_Desc/Copy)*

7.  Select a category in the **Copy to Category** list box.
    
    **NOTE**: The list box displays all categories in Integrate.

8.  Enter a name in **Copy to Process**.
    
    **NOTE**: This name must be unique. The name can contain all letters
    (A-Z), all numbers (0-9), and underscores. It cannot contain special
    characters. Integrate will replace special characters with
    underscores in the copied process name.
    
    <span style="font-weight: bold;">NOTE</span>: This field is required
    to perform the copy.

9.  Enter a description in <span style="font-weight: bold;">Copy to
    Process Description</span>.

10. Click **Save**.

11. Click **Execute**.
    
    <span style="font-weight: bold;">NOTE</span>: This button is
    disabled until required fields are completed.

The process is added to the category.
