+++
title = 'Images H'
solution = 'Platform'
+++

# Images H

[Images V](#Images)

<div class="use">

Use this page to [Add an Image to the
DSP®.](../Use_Cases/Add%20an%20Image%20to%20the%20DSP)

</div>

To access this page, select **Admin \> Configuration \> Style \>
Images** in the *Navigation* pane.

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>IMAGE NAME</p></td>
<td><p>Displays the named space name of the image.</p>
<p><strong>NOTE</strong>: Images are named using a name space, two or more namesseparated by a period. Each part must begin with a letter, and cannot contain spaces or punctuation. Names can contain letters or numbers.</p>
<p><strong>NOTE</strong>: When the image is uploaded, this name replaces the file name of the uploaded image. For example, if the image name is up.arrow and the file to be uploaded is called Bluearrow.jpg, the uploaded file is renamed to up.arrow.jpg.</p>
<p><strong>NOTE</strong>: The name space must not begin with any delivered WebApps' name space. If the new Image record does begin with a delivered WebApp's name space, an error message displays when a user attempts to save it.</p></td>
</tr>
<tr class="odd">
<td><p>IMAGE</p></td>
<td><p>Displays the image.</p></td>
</tr>
<tr class="even">
<td><p>FILE LOCATION</p></td>
<td><p>Displays the path on the application server where the image was uploaded.</p></td>
</tr>
<tr class="odd">
<td><p>LOCATION</p></td>
<td><p>Click to upload the image file.</p></td>
</tr>
</tbody>
</table>

## <span id="Images"></span>Images V

[Images H](#)

<table>
<colgroup>
<col style="width: 50%" />
<col style="width: 50%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>Image Name</p></td>
<td><p>Displays the named space name of the image.</p>
<p><strong>NOTE</strong>: Images are named using a name space, two or more names separated by a period. Each part must begin with a letter, and cannot contain spaces or punctuation. Names can contain letters or numbers.</p>
<p><strong>NOTE</strong>: When the image is uploaded, this name replaces the file name of the uploaded image. For example, if the Image Name is up.arrow and the file to be uploaded is called Bluearrow.jpg, the uploaded file is renamed to up.arrow.jpg.</p></td>
</tr>
<tr class="odd">
<td><p>Image</p></td>
<td><p>Displays the image.</p></td>
</tr>
<tr class="even">
<td><p>Location</p></td>
<td><p>Displays the path on the application server where the image was uploaded.</p></td>
</tr>
<tr class="odd">
<td><p>Include in Sprite</p></td>
<td><p>If enabled, the image is included in the image sprite that is built to represent icons used in applications. When images are placed into one larger image, multiple images are moved in one transfer to the client. Then, the correct piece of that larger image is spliced and shown on the button, image column, or other places in the application.</p>
<p>Putting something in the sprite could help load times, but it would likely be minimal considering how few images most clients use.</p>
<p><strong>NOTE</strong>: An image sprite can be used for application development scenarios for dspConduct™, Construct or custom WebApps.</p></td>
</tr>
<tr class="even">
<td><p>System Image</p></td>
<td><p>If checked, the image is delivered as part of the installation. If unchecked, this image was added by a user. This check box cannot be updated.</p></td>
</tr>
<tr class="odd">
<td><p>Legacy Name</p></td>
<td><p>Displays the name of the image if the image was used in an older version of the platform.</p></td>
</tr>
</tbody>
</table>
