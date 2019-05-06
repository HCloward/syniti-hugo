# Add an Image to the DSP®

An Administrator can add an image to the DSP® that can be used in
delivered WebApps and custom WebApp pages wherever images can be set.

**NOTE:** Custom images are retained during an upgrade. Updates to
delivered images are overwritten.

**NOTE:** The images delivered on WebApp pages cannot be modified.

Images can be added to:

  - [Page columns for custom
    pages](../../WebApp_Dev/Link_to_a_Page_Using_Buttons_and_Images.htm)
  - [A menu in a custom
    WebApp](../../WebApp_Dev/Add_a_Menu_to_the_Navigation_Pane.htm)
  - [Quick Links](Create_Quick_Links_by_Role.htm)
  - The *[Request
    Status](../../../Master_Data_Mgmt/dspConduct/Page_Desc/Request_Status.htm)*
    page in dspConduct™ when adding a custom status. Refer to [Add a
    Custom Request
    Status](../../../Master_Data_Mgmt/dspConduct/Use_Cases/Add_a_Custom_Request_Status.htm)
    in dspConduct™ for more information.
  - A custom mapping status or rule status n Map. Refer to [Configure
    Mapping Status and Rule
    Status](../../../Migration/Map/Use_Cases/Mapping_Status_and_Rule_Status.htm#Configure_Mapping_Status_and_Rule_Status)
    in Map for more information.
  - A request status in dspCompose™. Refer to [Configure Request
    Statuses](../../../Data_Quality/dspCompose/Config/Configure_Request_Statuses.htm)
    in dspCompose™ for more information.
  - [Custom Links on a page](Add_a_Custom_Link.htm)

The maximum file size for an uploaded image is defined by the
maxRequestLength value in the web.config file.

Refer to [Add or Update Custom Icons for Custom
WebApps](Add%20or%20Update%20Custom%20Icons%20for%20Custom%20WebApps.htm)
for information about adding svg images.

To add an image:

1.  Select **Admin \> Configuration \> Style \> Images** in the
    *Navigation* pane.

2.  Click **Add**.
    
    *[View the field descriptions for the Images
    page](../Page_Desc/Images%20H.htm)*

3.  Enter a unique image name with at least two parts separated by a
    period in the **IMAGE NAME** field.
    
    **NOTE:** Image are named using a name space, two or more names
    separated by a period. Each part must begin with a letter, and
    cannot contain spaces or punctuation. Names can contain letters or
    numbers.
    
    **NOTE:** When the image is uploaded, this name replaces the file
    name of the uploaded image. For example, if the Image Name is
    up.arrow and the file to be uploaded is called Bluearrow.jpg, the
    uploaded file is renamed to up.arrow.jpg.

4.  Click **Save**.

5.  Click the **Location** icon for the new record.

6.  Upload the image.

This image is available to select from the IMAGE ID list box anywhere it
displays in the product.
