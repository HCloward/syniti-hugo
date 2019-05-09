+++
title = 'Consolidation'
solution = 'Platform'
+++

# Consolidation

Another problem is making sure you choose the most appropriate control
mechanism to achieve the end goal. Most individual mechanisms can
implement the same behavior in one way or the other. However, some may
require much less computational logic.

An example of this is that a DCV can contain a boaUserID, which can
allow for a cell to be controlled exclusively off of the boaUserID. For
instance:

<span style="font-family: &#39;Courier New&#39;;">SELECT
boaUserSel.\[UserID\] as
boaUserID,</span>

<span style="font-family: &#39;Courier New&#39;;">\[Table\].\[KeyField\],</span>

<span style="font-family: &#39;Courier New&#39;;">CASE WHEN
boaUserSel.\[UserID\] like ‘a%’ THEN 1 ELSE 0 END as
\[ControlledField\]</span>

<span style="font-family: &#39;Courier New&#39;;">FROM \[Table\] CROSS
JOIN boaUserSel</span>

<span style="font-family: &#39;Courier New&#39;;">Instead of a DCV, this
should be a UCV, which would reduce the logic to</span>

<span style="font-family: &#39;Courier New&#39;;">SELECT
boaUserSel.\[UserID\] as boaUserID,</span>

<span style="font-family: &#39;Courier New&#39;;">‘ControlledField’ as
boaColumn,</span>

<span style="font-family: &#39;Courier New&#39;;">CASE WHEN
boaUserSel.\[UserID\] like ‘a%’ THEN 1 ELSE 0 END as
\[boaControlStatus\]</span>

<span style="font-family: &#39;Courier New&#39;;">FROM boaUserSel</span>

This would result in the pages performance scaling linearly against the
applications User count, as opposed to a multiplication of Users \*
Table Data.
