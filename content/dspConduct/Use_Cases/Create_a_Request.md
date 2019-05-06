# Create a Request

Requests are created in dspConduct™ when a new request is added and
saved on a task page in the Content WebApp. For requests to be created,
a user must configure the Content WebApp page to communicate with
dspConduct™ to pass request data from the Content WebApp to dspConduct™.
Configuration is also needed when certain request statuses are updated
in the Content WebApp. Refer to [Manage Request
Statuses](../Config/Manage_Request_Statuses.htm) for more information
about statuses in dspConduct™.

Refer to [Auto-generate Request-related
Objects](Auto_Generate_Request_related_Objects.htm) for information
about creating tables, views and stored procedures in the Content WebApp
automatically.

When a request is created, the request status is “Draft.” When a Content
user submits the request, stored procedures change its request status to
“Request in Process,” and dspConduct™ Request Roles for the request
become available for processing.

<span style="font-weight: bold;">NOTE</span>: For new requests that are
automatically created as part of a multi-scenario business process, the
Content Request page OnValidate event is automatically executed. The
Cransoft UserID 'process' must have access to the Content Request page
in order to execute the OnValidate event.
