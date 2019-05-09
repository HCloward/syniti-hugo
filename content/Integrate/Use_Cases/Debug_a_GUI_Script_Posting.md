+++
title = 'Debug a GUI Script Posting'
solution = 'Platform'
+++

# Debug a GUI Script Posting

Sometimes the best way to determine a problem with a post is to manually
step through the post process and examine each step in the post with the
actual data being processed. Integrate provides a mechanism to enable
this manual step-through processing: GUI Debug Script creation for GUI
script postings.

It may also be helpful to review the script for the entire record set
prior to uploading.

There are two debugging methods:

  - **Create GUI Debug Script** is used for debugging individual records
    that have posted and failed. The script is created<span> </span>a
    single record at a time and stops running when a record fails.
  - **Create Full GUI Debug Script** does not attempt to
    upload<span> </span>records, but generates the script for an entire
    record set. Use this method to check the script logic prior to
    uploading.

Each debugging method has its strengths so it is wise to choose
accordingly depending on the debugging situation.

### Debug with the Create GUI Debug Script

If the **Create GUI Debug Script** check box is enabled on the
**Advanced** tab of the *Process Post* page’s *Vertical* View, Integrate
creates a copy of the actual GUI script run against SAP and writes it to
the ttMessage table in Integrate in the GUIDebugScript column along with
the results of the post. This script can be downloaded from the
*Messages* page and run directly in the SAP GUI, allowing a step-by-step
walkthrough of the post process.   

**NOTE:** If using the **Create GUI Debug Script** option for a process
with multiple templates that contain a GUI Script template, use the
**Start Template Priority** and **End Template Priority** fields to
restrict the posting to the GUI Script template only. For example, if a
multi-template process contains a GUI Script template with a priority of
30, and the **Create GUI Debug Script** option is to be used, enter 30
in the **StartTemplate Priority** and **End Template Priority** fields
on the **Advanced** tab of the *Process Post* page’s *Vertical* View.
When posting the process, Integrate will only post the GUI Script
template, and the steps in this section can be used. Refer to [Post a
Process with Multiple
Templates](Post_a_Process_with_Multiple_Templates) for more
information.

To debug the GUI script, generate the VB script file and run the
recording in the SAP GUI. Refer to [Record a GUI
Script](Record_a_GUI_Script) for more information.

To view the VB script file from Integrate:

1.  Select **Categories** from *Navigation pane*.

2.  Click the **Processes** icon for a category.

3.  Click the **Postings** icon for a process.

4.  Click **Messages** for the posting.

5.  Locate the process post that uses the GUI script.

6.  Click **Debug**.
    
    **NOTE**: In Chrome, a page opens that displays the script. The
    script can be copied from this page.  
    In Internet Explorer, a *Save* dialog box displays with the name of
    the script with a .vbs extension. Save the VB script file to view
    it.

To run the recording in the SAP GUI:

1.  Log in to the SAP GUI.
2.  Click the **Customize Local Layout** icon.
3.  Select **Script Recording And Playback**.
4.  Click **Play** .
5.  Browse to the VBScript file.
6.  Select **Open**; the SAP GUI walks through the post process in real
    time.

### Debug with the Create Full GUI Debug Script

To generate the script for the entire record set to debug before records
are uploaded:

1.  Create the GUI script. Refer to [Record a GUI
    Script](Record_a_GUI_Script) for more information.
2.  Select **Categories** from *Navigation pane*.
3.  Click the **Processes** icon for a category.
4.  Click the **Postings** icon.
5.  Click **Vertical View** for a process post that uses a template
    based on a GUI script.
6.  Click **Advanced** tab.
7.  Click **Create Full GUI Debug Script**.
8.  Click **Download Full GUI Debug Script**.

**NOTE**: Depending on the browser and browser settings, the VB script
may open or the user may need to confirm that the VB script file should
be opened.
