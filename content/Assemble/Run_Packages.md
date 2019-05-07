+++
title = ''
solution = 'Platform'
+++

# <span>Run Packages</span>

Once source and target information is configured and tested, the
CranPort package can be run. A package is run in the background,
enabling the user to continue to navigate through the WebApp. Columns
are automatically created during the run process. If target sources
already exist when the package is executed, any existing data is
deleted.

To run a package:

1.  Select **Packages** in the *Navigation* pane.

2.  Locate the Package Name.

3.  Click the **Run** icon for the **PACKAGE NAME**.

4.  Click the **Run** icon; a confirmation message displays.

5.   Click **Yes**; a background job is submitted for the package.
    
    **NOTE:** The package submissions are always placed into a queue.
    The speed in which they get picked up depends on what the user chose
    for the QueueID. If the specific Queue is not under heavy usage, it
    will usually be fairly quick (few seconds).

6.  Click **Logs** button to view the status of the package.
