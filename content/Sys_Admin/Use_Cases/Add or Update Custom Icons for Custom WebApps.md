+++
title = 'Add or Update Custom Icons for Custom WebApps'
solution = 'Platform'
+++

# Add or Update Custom Icons for Custom WebApps

An Administrator can add images to the DSP and use them as icons in
custom WebApps. Refer to [Add an Image to the
DSP](Add%20an%20Image%20to%20the%20DSP) for detailed information.

**NOTE**: When adding an image, you cannot use the name of an image
delivered with the DSP. Additionally, you cannot use the namespace of a
delivered WebApp, such as CranSoft, when creating images.

With 7.0, icons have been changed to .svg format. These new images are
included in the DSP, and you can update images in custom WebApps to use
these new images.

On the *[Images](../Page_Desc/Images%20H)* page, search for "svg" in
the quick search to display the new images.

You can still create and use non-.svg images (such as .png or .gif) as
in previous versions.

To add .svg images, follow these guidelines.

  - Images are rendered in the grid as 24 x 24 pixels.
  - .svg images require two image files, one for a dark image and one
    for a light one.
      - Add the path to the dark image (for example,
        Images/CustomWebAppName/MySVGImage.svg) in the Location field on
        the *Vertical* View of the *Images* page.
      - Create the light image, and save it to the same folder as the
        dark image on the WebApp server. Use the naming convention
        XXXXX\_highcontrast.svg where XXXXX is the same name used in the
        dark image (for example, MySVGImage\_highcontrast.svg). The DSP
        uses the dark and light images depending on the style the user
        selects and the background color behind the image. Foreground
        and background colors are set on the
        [Styles](../Page_Desc/Styles_H) page. Refer to [Add a
        Style](Add_a_Style) for more information.

**NOTE**: Custom images are retained during an upgrade. Updates to
delivered images are overwritten.
