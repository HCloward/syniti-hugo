+++
title = 'Help with Command Timeouts'
solution = 'Platform'
+++

# Help with Command Timeouts

Command timeouts are possible in all areas of the DSP. If interfaces,
events or validations are timing out, try these two solutions:

  - Increase the Connection Timeout for the InterfaceServer Data Source.
    Do not increase beyond 3500 seconds.
  - Check the timeout settings for the Data Sources used in the events.
    Do not increase beyond 3500 seconds.

Timeout settings are set on the *[Data
Sources](../../Sys_Admin/Page_Desc/Data_Sources_HSysAdmi.htm#Advanced_Properties_Tab)*
page on the Advanced Properties tab in System Administration.
