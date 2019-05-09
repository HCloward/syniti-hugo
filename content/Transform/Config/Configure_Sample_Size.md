+++
title = 'Configure Sample Size'
solution = 'Migration'
+++

# Configure Sample Size

A sample size is used with a sampling method on Target audit reports to
set the number of random rows to be verified by users. This process
allows a certain number of rows from very large Targets to be selected
at random for quality verification prior to, or subsequent to, a data
load.

Users should decide from an auditing perspective what sample size is
acceptable and choose the method that will give them that sampling size.
For example, if users select method ANSI/ASQC Z1.4 GI III and have 4500
records then they will get 315 records, but if they choose ANSI/ASQC
Z1.4 S-2, they would only get 8 records. To find out the number or
records that will be returned for a method navigate to **Sample Methods
(Setup) \> Sample size (report icon)**.

If the provided sample sizes do not produce the number of records that
you need, you can create your own.

Sample sizes delivered with the platform cannot be edited, but a sample
size can be added. To modify a sample size, delete the record and add a
new one.

To add a sample size in Transform:

1.  [Access Transform](Access_Transform).

2.  Select **Configuration \> Setup \> Sampling Methods(Setup)** in the
    *Navigation* pane.

3.  Click the **Sample Size** icon next to the sampling method you want
    to use. For example, ANSI/ASQC Z1.4 GI I or Square Root.
    
    **NOTE:** This is the method used in Transform if it meets auditing
    requirements.
    
    **NOTE:** Using the number of records in your table, locate the
    range that it falls between. The sample size will determine how many
    sample records will be returned.

4.  Click **Add**.
    
    *[View the field descriptions for the Sample Sizes (Setup)
    page.](../Page_Desc/Sample_Sizes_Setup)*

5.  Enter a value in the **RANGE LOW** field.
    
    **NOTE:** The value entered for RANGE LOW must be smaller than the
    number of records in the table.

6.  Enter a value in the **RANGE HIGH** field.
    
    **NOTE:** The value entered for RANGE HIGH must be larger than the
    number of records in the table.

7.  Enter a value in the **SAMPLE SIZE** field.
    
    **NOTE:** This is the number of records to return based on the
    low/high range and is a hard-required field.

8.  Enter text in the **COMMENT** field.

9.  Click **Save**.
