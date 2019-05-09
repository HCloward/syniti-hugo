+++
title = 'Stop and Start Service Pages'
solution = 'Platform'
+++

# Stop and Start Service Pages

There are no security restrictions for stopping or starting a service
page. If the user has access to the
<span style="font-style: italic;">Service Pages</span> page, they can
start/stop at will.

Once the service page has begun processing, it cannot be stopped – the
Stop button is disabled. If a service page is started accidentally, the
user will only be able to stop it while it is in queue.

Notifications will not be sent to any user when service pages are
stopped or started. 

To stop or start a service page:

1.  Select **Resources \> Service Pages** in *Navigation* pane.
    
    **NOTE**: A list of all service pages, active and inactive, displays
    for all WebApps.

2.  Either:
    
      - Click **Start** for the **WEB APP** to start the service page.
    
    **NOTE**: The service page is queued to run as soon as possible. The
    Start icon is disabled and the Stop icon is enabled. The Stop button
    will then be disabled when processing had begun.
    
    OR
    
      - Click **Stop** for the **WEB APP** to stop the service page
    
    **NOTE**: The service page will not stop if it is already running.
    It will only stop while in queue. The service page will run again
    according to the frequency set on the Service Properties tab on the
    *Page* page’s Vertical View (WebApps \> Pages \> Vertical View for a
    page with Page Type of Service). Refer to [Configure Service
    Pages](Configure_Service_Pages.htm) for more information.
    
    **NOTE:** A Page Designer creates a service page. Refer to [Create a
    Service Page](../../WebApp_Dev/Create%20a%20Service%20Page.htm) for
    more information.
