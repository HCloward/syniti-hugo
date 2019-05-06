# BDC Script and GUI Script Recording Tips

A recording should be as perfect as possible. It should not have any
errors messages and there should only be warning messages when
necessary. If a mistake is made while entering data, stop recording and
try again.

The following tips help facilitate script recording:

  - When recording, do not use the scroll bars, cursor keys or the mouse
    to change the position because these actions do not get recorded.
    Successful recordings need to be done with the **Page Down** key.
  - For efficiency, do not hit the **Enter** or the **Return** key
    unless it is absolutely necessary.  
  - There are three ways to mark a field as *touched*: 
      - Add a space to the end and delete it.
      - Delete the value and re-type it.
    <!-- end list -->
      - Change the value completely.
  - Be careful when selecting views. The data being recorded may require
    more or fewer views than other data. If this is the case, view
    selections may not be synchronized with the recording and cause the
    wrong views to be selected during the post. Avoid this issue by
    selecting all views, even if all views will not be used.
  - When the header information has been entered on a multi-line
    transaction, it is good practice to force a screen break to separate
    the header and line item screens. This practice make it easier to
    identify where the header information ends and the line item detail
    begins. To force a screen break, press the Enter key.
  - It is important to know the transaction and the required data before
    the recording process starts.
  - Record generically. The transaction must work for all objects, such
    as material types in materials or account groups in customers.
  - Keep the number of screens to a minimum. For example, click **Save**
    rather than having the transaction ask to save. Avoid using list
    boxes. Know the transaction and what information is used to populate
    the fields prior to executing the recording.
  - Populate as many fields as necessary to map in the recording.
    Missing fields can be added later to the script, but it is better to
    record the fields needed.
  - If the SAP screen includes a table, look for a way to move to the
    end of the table to enter the data in the same field subscript on
    the screen, either line one or two. Often, there is a **New Line**
    button available to move the table and position the cursor at the
    end. If this button fails, insert the data on the bottom line and
    move it up to the first free line.
  - Recordings should
    **<span class="underline"><span style="color: #ff0000;">not</span></span>**
    be saved in the same directory that the platform will later save the
    file once it is imported. Saving the recording as an imported file
    in the same directory can cause an error or duplicate file.
  - Ensure the language for fields in the view (e.g., UOM) matches the
    default SAP language for the SAP login.
  - Ensure the number and date formats in the view match the format in
    the SAP login.
  - **Special Rules for MM01** – Be careful using the MM01 transaction.
    Different materials types may have the views assigned in different
    sequences. If needed, go to the second page and replace **Enter** on
    the recording of that page with **P++**. This replacement causes a
    page to appear at the bottom of the selection window.
  - **Special Rules for MM02** – When changing a view,
    **<span class="underline"><span style="color: #ff0000;">always</span></span>**
    select the basic view first. Use the list box on the right side of
    the screen to locate the views that are to be changed. The views set
    up for the given material determine the contents of the list box. Do
    not record a direct selection to the view to be changed.
  - For Customer and Vendor add or update transactions, the user is able
    to select the desired views; selection fields are not configurable.
