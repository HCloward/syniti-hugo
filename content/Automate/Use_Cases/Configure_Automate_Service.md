# Configure Automate Service Pages

Automate uses Service pages for background processing. It is recommended
to adjust the schedule of these Service pages for smoother and more
efficient interface processing.

Users must have access to System Administration in order to configure
Automate Service pages.

Service pages include:

  - [Instance Trim](#InstanceTrim)
  - [Interface (Handle Service Drops)](#InterfaceHSD)
  - [Site Maintenance](#SiteMaintenance)
  - [Interface (Initiator)](#InterfaceInitiator)
  - [Interface (Retry)](#InterfaceRetry)

To configure a service page’s schedule:

1.  Select **Admin \> WebApps** in the *Navigation* pane.

2.  Click the **Pages** icon for the InterfaceServer WEB APP NAME.
    
    **NOTE:** Automate is formerly known as “InterfaceServer” and some
    references to this old name are in System Administration.

3.  Click **Vertical View** for a PAGE TYPE of Service.

4.  Click the **Service Properties** tab.

5.  Click **Edit**.
    
    [View the field description for the Service Properties tab the Pages
    page’s Vertical
    View](../../Sys_Admin/Page_Desc/Pages_H.htm#ServiceAdvPropstab)

6.  Enter a new value in the **Service Qty** field.

7.  Select a new UOM from the **Service UOM** list box.

8.  Click **Save**.

## <span id="InstanceTrim"></span> Instance Trim

**Description:** Deletes all History records that were older than what
is defined in the History Retention days on the
*[Parameters](../Page_Desc/Parameters.htm)* page. For example, if the
History Retention is set to 30, any History records older than 30 days
are deleted.

**Default Schedule:** Once daily (Service Qty is set to 1 and Service
UOM is set to Day(s)).

**Recommended Schedule:** The default schedule is fine to use.

## <span id="InterfaceHSD"></span> Interface (Handle Service Drops)

**Description:** Checks to see if there are any interface jobs that
failed in the job queue (in this case, due to the DSP service stopping),
but are still in a running state in Automate.

**Default Schedule:** Every 2 minutes (Service Qty is set to 2 and
Service UOM is set to Minutes(s)).

**Recommended Schedule:** Every 10 minutes (Service Qty is set to 10 and
Service UOM is set to Minutes(s)) at a minimum because if the
DSP service stops, the service will take a few minutes to come back up
and mark all the jobs as "failed."

## <span id="SiteMaintenance"></span> Site Maintenance

**Description:** Deletes old records out of the Trace Logs records (when
Debug Mode is enabled on the *Vertical* View of the
*[Interfaces](../Page_Desc/Interfaces.htm#InterfacesV)* page), and the
Logical Path list of folders and file records (located on the *[Logical
Path Instance (Browse)](../Page_Desc/Logical_Path_Instance_Browse.htm)*
page.

**Default Schedule:** Once daily (Service Qty is set to 1 and Service
UOM is set to Day(s)).

**Recommended Schedule:** The default schedule is fine to use.

## <span id="InterfaceInitiator"></span> Interface (Initiator)

**Description:** Submits any Interfaces that are currently due to run.
When an Interface is picked up to run, a new job is added to the Job
Queue called ProcessBackground, which actually runs the Automate events
for that interface.

**Default Schedule:** Every 30 seconds (Service Qty is set to 30 and
Service UOM is set to Second(s)).

**Recommended Schedule:** Every 2 minutes (set Service Qty to 2 and
Service UOM to Minute(s)). If an Automate interface is set to run every
hour, that job may wait for 2 minutes before getting submitted,
depending on when the last time the Service page was run.

## <span id="InterfaceRetry"></span> Interface (Retry)

**Description:** Picks up any Automate jobs that have paused due to a
Retry set up in a validation for one of the Automate events.

**Default Schedule:** Every 30 seconds (Service Qty is set to 30 and
Service UOM is set to Second(s)).

**Recommended Schedule:** Every 2 minutes (set Service Qty to 2 and
Service UOM to Minute(s)). If an Automate interface is set to run every
3 minutes, that retry may sit for 2 minutes before getting submitted.
