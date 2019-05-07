+++
title = 'Create a Final Finish Where Clause for a CranPort Package'
solution = 'Data Quality'
+++

# Create a Final Finish Where Clause for a CranPort Package

<span style="font-weight: bold;">NOTE</span>: A table or a view that
resides in a specified data source is used to provide data values for
the Where clause.

<span style="font-weight: bold;">NOTE</span>: If the table has multiple
keys, build a Where clause for each key. When the Where clause is built,
the key values are concatenated.

Refer to [Configure Data Download During the Final Finish Process to use
a CranPort
Package](Configure_Data_Download_During_the_Final_Finish_Process_to_use_a_CranPort_Package.htm)
for general information.

To build a Where clause for the CranPort package used to download the
data to the target table:

1.  Click <span style="font-weight: bold;">dspConduct \> Design</span>
    in the *Navigation* pane.

2.  Click the **Tasks** icon for a category.

3.  Click the **Final Finish Tables** icon for a main parent task.

4.  Click **Vertical View** for a table.

5.  Click the **Where Clause Builder** icon.

6.  Select the column name from the table that contains the mapped value
    to build the Where clause in the **COLUMN NAME** list box.

7.  Select the data source that contains the table or view in the **DATA
    SOURCE ID** list box.

8.  Select the table or view name in the **TABLE VIEW NAME** list box.
    
    **NOTE:** The table or view must already exist in the data source.

9.  Select the value used in the Where clause in the **MAPPED VALUE**
    list box.
    
    **NOTE:** The default Where clause ((\#ColumnName\# IN (\#Data\#)))
    can be modified if needed.

10. Click **Save**.
