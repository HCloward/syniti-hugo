# Extract RFC Functions

Integrate supports the execution of any RFC-enabled Function Module in
SAP, including the execution of RFCs and the posting of data via BAPIs.

Before creating a BAPI/RFC template, a Template Administrator must
extract the list of RFC functions and their descriptions enabled in the
SAP system using the <span style="font-style: italic;">[Data Source
Registry](../../Common/Page_Desc/Data_Source_Registry_H.htm)</span> page
in Common.

Integrate pulls the definition of the Function Module from SAP to
complete the template.

To extract RFC functions in Common:

1.  Select <span style="font-weight: bold;">Configuration \> Data Source
    Registry</span> in the
    <span style="font-style: italic;">Navigation</span> pane.

2.  Click <span style="font-weight: bold;">Vertical View</span> for the
    data source with an <span style="font-weight: bold;">APPLICATION
    DATA SOURCE TYPE</span> of SAP Application Server,

3.  Click the <span style="font-weight: bold;">RFC Extract</span> icon.
    
    **NOTE:** RFCs must be extracted before the first BAPI/RFC template
    type can be created.

4.  Click the <span style="font-weight: bold;">RFC Functions</span> icon
    to view the list of RFCs enabled in the SAP System and their
    descriptions.
