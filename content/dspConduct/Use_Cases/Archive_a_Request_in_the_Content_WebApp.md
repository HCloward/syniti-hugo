+++
title = 'Archive a Request in the Content WebApp'
solution = 'Master Data Management'
+++

# Archive a Request in the Content WebApp

To archive request data, the Designer creates a process in the Content
WebApp that must execute the dspConduct™ stored procedure
apiArchiveRequest to archive the corresponding dspConduct™
Request-related table data into dspConduct™ archive tables.

Register this stored procedure within the archiving process of the
Content WebApp. The dspConduct™ stored procedure apiArchiveRequest
expects parameters RequestID and WebAppID.  This stored procedure must
only be executed for specific RequestIDs whose request status marks them
as eligible to be
archived.

<span style="font-weight: bold;" data-xmlns="http://www.w3.org/1999/xhtml">NOTE</span>:
This stored procedure checks the status of the RequestID against the
Category's Request Status Days Active for the status. If that check does
not indicate that the Request is ready to be archived (i.e., the number
of days active for the status has not passed), the Request-related table
data is NOT removed from dspConduct™.

After a request is archived, as a part of the Content WebApp’s process
that deletes data from tt tables, the dspConduct™stored procedure
apiDeleteRequestAfterArchive must be executed to delete the dspConduct™
Request-related table data from dspConduct™ tt tables.

dspConduct™ stored procedure apiDeleteRequestAfterArchive expects
parameters RequestID and WebAppID.
