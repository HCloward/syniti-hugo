+++
title = 'Manage Element Documentation'
solution = 'Master Data Management'
+++

# Manage Element Documentation

The Element Documentation page supports the uploading and downloading of
documents for elements. Each element page has a link to the [Element
Documentation](../Page_Desc/Element_Documentation.htm) page. Elements
that allow adding documents are:

  - Business Process
  - Scenario
  - Role
  - Task
  - Scenario Role
  - Scenario Role Task

Only one document can be uploaded at a time. The upload process stores
the document in a unique area and provides file properties to the new
file. Once the document is uploaded, a Replace File icon is enabled. If
an element document already exists, the ability to upload on this page
is disabled and the Replace File icon is enabled. Refer to [Upload and
Download Element
Documentation](Upload_and_Download_Element_Documentation.htm) for more
information.

<span style="font-size: 11.0pt;color: #333333;font-weight: bold;">NOTE:</span>
The Path value of data source DGE\_ElementDocument\_FilePath is the
"root" of the path where all Element Documents are stored on the web
server. This data source path value must be populated for documents to
be uploaded successfully. This path value should have been populated by
the Administrator when dspConduct™ was installed.  The complete document
path is made up of the value from DGE\_ElementDocument\_FilePath Path +
value of Element + value of ElementID.

Topics covered are:

  - [Upload and Download Element
    Documentation](Upload_and_Download_Element_Documentation.htm)
  - [Replace an Element Document](Replace_an_Element_Document.htm)
  - [Generate Element Documents](Generate_Element_Documents.htm)
