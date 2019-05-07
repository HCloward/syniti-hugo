+++
title = 'No batch input data for screen'
solution = 'Platform'
+++

# No batch input data for screen

This error indicates that there was a screen that appeared during the
post that was not in the recording. Sometimes the data used for the post
sends SAP in a different path of screens than the data used in the
recording. For example, some data may require a plant number to be
entered. If a plant number is not entered during the recording, some
records may fail. The solution is to force the screen to come up in the
recording and to set conditions on the screen depending on what data is
used.
