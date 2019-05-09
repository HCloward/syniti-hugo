+++
title = 'Create Column Dictionaries'
solution = 'Platform'
+++

# Create Column Dictionaries

Each column can be assigned a dictionary. A dictionary contains words
and their synonyms. Dictionaries can be used to resolve abbreviations,
for example, St to Street, or nick names to full names. Dictionaries can
also be used to normalize common industry or company-specific
abbreviations into strings.

Dictionaries are a powerful feature, but should be used sparingly. Each
word in the dictionary is stored in the index and increases the index
size, which negatively impacts the search performance.

To create a dictionary:

1.  Select **Configuration \> Search \> Dictionaries** in the
    *Navigation* pane.

2.  Click **Add**.
    
    [View the field descriptions for the Dictionaries
    page.](../Page_Desc/Dictionaries)

3.  Enter a name for the dictionary in **DICTIONARY** field.

4.  Click **Save**.

5.  Click **Words** for the dictionary.
    
    **NOTE**: Because this is a new dictionary, the page displays in add
    mode.
    
    *[View the field descriptions for the Dictionary Words
    page](../Page_Desc/Dictionary_Words)*.

6.  Enter a value in the **WORD** field.

7.  Enter a value in the **SYNONYM** field.
    
    **NOTE**: The WORD or SYNONYM can be used in multiple combinations,
    but each WORD-SYNONYM combination must be unique.

8.  Click **Save**.
