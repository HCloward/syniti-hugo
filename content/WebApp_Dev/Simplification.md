+++
title = 'Simplification'
solution = 'Platform'
+++

# Simplification

The biggest performance gains most often come from SQL simplifications.
Becoming a SQL expert will be the best way to ensure complex pages will
perform at their best.

For example, the following view:

SELECT boaUserSel.\[UserID\] as boaUserID, ‘ControlledField’ as
boaColumn, CASE WHEN boaUserSel.\[UserID\] like ‘a%’ THEN 1 ELSE 0 END
as \[boaControlStatus\] FROM boaUserSel

Could be:

 

SELECT boaUserSel.\[UserID\] as boaUserID, ‘ControlledField’ as
boaColumn, 1 as \[boaControlStatus\] FROM boaUserSel where
boaUserSel.\[UserID\] like ‘a%’
