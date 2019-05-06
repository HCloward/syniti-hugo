# Updates to Finishing a Data Role for Templates with the Security View

The Data role is finished differently if:

  - The template uses Org Units and

  - Users have been assigned to different Org Unit Values and

  - The Org Unit security view has been added to the template.

In this case, the Finish button will not dither and the Data role will
not be finished until the Data role for all Org Unit Values has been
finished. In other words, a user assigned to each Org Unit Value must
finish the Data role for the request before the request can move to the
Review role. Until this condition is met, the Finish button will be
active.

For example, a template has the Org Unit North American Plants assigned.
User A is assigned to Plant A. User B is assigned to Plant B. User C is
assigned to Plant C and Plant D.

A Template Administrator adds the security view and boaUserID to the
<span style="font-style: italic;">Horizontal</span> View of the Data
Entry pages, and creates a request based on the template. The Template
Administrator reviews the Org Units assigned to the request, and removes
the Org Unit Value Plant D from the request. Once the Org Units are
confirmed, the request is active.

User A enters data manually for Plant A, then clicks Finish on the
<span style="font-style: italic;">Request (Roles)</span> page.

The Finish button remains active, and the Data role is not finished.

User B enters data and clicks Finish on the
<span style="font-style: italic;">Request (Roles)</span> page.

The Finish button remains active, and the Data role is not finished.

User C enters data for Plant C and clicks Finish on the
<span style="font-style: italic;">Request (Roles)</span> page.

The Finish button is disabled, and the Data Role is finished. The
request moves to the Review role.

<span style="font-weight: bold;">NOTE</span>: If a Template
Administrator does not add the security view to the template, when a
user clicks Finish for the Data role on the
<span style="font-style: italic;">Request (Roles)</span> page, all
requests for all Data roles will be marked as finished and the request
will move to the Review role. Continuing the example above, if the
Template Administrator had not added the security view to the
<span style="font-style: italic;">Horizontal</span> View for the Data
Entry pages, when User A clicks Finish on the
<span style="font-style: italic;">Request (Roles)</span> page, requests
for Plant B and C would also be marked as finished and move to the
Review role, even though User B and User C had not entered data for
their Org Unit Values.
