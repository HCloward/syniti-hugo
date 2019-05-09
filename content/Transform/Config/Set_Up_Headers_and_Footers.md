+++
title = 'Set Up Headers and Footers for Transform Reports'
solution = 'Migration'
+++

# Set Up Headers and Footers for Transform Reports

The headers and footers that display on Transform reports can be
customized in Console to include information that is generated when the
report is written to a file, such as generated date, total number of
pages, or path and file name. A user can also enter static text to
include in the header or footer.

How headers and footers display can also be customized in many ways.
Transform reports do not require headers or footers. Reports can also
have a header or footer only. Text or data can display in the left,
center or right of headers and footers, or in any combination of the
three.

The same headers and footers are used on all Transform reports, though
they can be updated at any time.

Use two pages in Console to set up headers and footers.

  - Use the *[Report Headers / Footers
    (Setup)](../../Console/Page_Desc/Report_Headers_Footers_Setup)*
    page to add the text or data to appear in the header and footer.

**NOTE:** Console allows a user to add multiple headers and footers.

  - Use the **Transform** tab on the
    *[Parameters](../../Console/Page_Desc/Parameters)* page to set
    the header and footer to use for reports.

The following values are available to use in headers and
footers:

|                |                                                                                                                                                                        |
| -------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Value          | Description                                                                                                                                                            |
| File           | Displays the file name of the report. Refer to [Naming Conventions](../Use_Cases/Naming_Conventions) for more information.                                         |
| File Date      | Displays the date the file was last saved.                                                                                                                             |
| File Time      | Displays the time the file was last saved.                                                                                                                             |
| Generated Date | Displays the date the report was generated in Transform.                                                                                                               |
| Page n of x    | Displays the current page and total number of pages in the report.                                                                                                     |
| Page number    | Displays the current page number.                                                                                                                                      |
| Path           | Displays the path where the report is stored, entered in the Report Path field on the Transform tab of the *Parameters* page in Console.                               |
| Path and file  | Displays the path where the report is stored and the file name of the report. Refer to [Naming Conventions](../Use_Cases/Naming_Conventions) for more information. |
| Sheet          | Displays the number of the sheet, used to differentiate a sheet that spans multiple pages from a page number.                                                          |
| Total pages    | Displays the total number of pages in the report.                                                                                                                      |

 

To add a header and footer in Console:

1.  Select **Advanced Configuration \> Report Headers / Footers
    (Setup)** in the *Navigation* pane.

2.  Click **Add**.
    
    [View the field descriptions for the Report Headers/Footers (Setup)
    page](../../Console/Page_Desc/Report_Headers_Footers_Setup)

3.  Enter a description of the header or footer in the **DESCRIPTION**
    field.
    
    **NOTE:** This description is selected on the Transform tab of the
    *Parameters* page when assigning the header and footer for Transform
    reports. Enter a meaningful description, especially if the header or
    footer should indicate the report contains confidential or
    proprietary information.

4.  Select an option in the **LEFT** combo box to indicate what data is
    left aligned in the header or footer  
    Or  
    Enter text in the **LEFT** combo box and click the **Use this
    value** link when complete.

5.  Select an option in the **CENTER** combo box to indicate what data
    is centered in the header or footer  
    Or  
    Enter text in the **CENTER** combo box and click the **Use this
    value** link when complete.

6.  Select an option in the **RIGHT** combo boxto indicate what data is
    right aligned in the header or footer  
    Or  
    Enter text in the **RIGHT** combo box and click the **Use this
    value** link when complete.

7.  Click **Save**.

To set the header and footer used in reports in Transform:

1.  Select **Advanced Configuration \> Parameters** in the *Navigation*
    pane.
2.  Click the **Transform** tab on the
    *[Parameters](../../Console/Page_Desc/Parameters)* page.
3.  Click **Edit**.
4.  Select a report description in the **Report Header** list box under
    Report Settings.
5.  Select a report description in the **Report Footer** list box under
    Report Settings.
6.  Click **Save**.

**NOTE:** The selected header and footer displays on all Transform
reports.
