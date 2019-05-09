+++
title = 'Automation Engine Action H'
solution = 'Platform'
+++

# Automation Engine Action H

[Automation Engine Action V](#Automation_Engine_Action1)

<div class="use">

Use this page to [Modify Actions](../Use_Cases/Modify_Actions).

</div>

To access this page, select <span style="font-weight: bold;">Common \>
Automation Engine \> Automation Engine Action</span> in
<span style="font-style: italic;">Navigation</span>
pane.

|              |                                                                                                                                                                                                                                       |
| ------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Field        | Description                                                                                                                                                                                                                           |
| ACTION       | Displays the Action in a DSP® component that calls the AE Task or Task Group stored in the AEID.  This field is not editable and the value is set by the software developers. It aligns with a specific event in one or many modules. |
| AEID         | Displays the AE Task or Task Group that is executed when the event specified by the Action is executed.  By changing this value, the action that runs for an event in a module can be modified.                                       |
| DSP SUPPLIED | If enabled, this content is delivered content provided by BackOffice and cannot be edited. If disabled, the content was added by the user. This setting cannot be updated from within Common.                                         |

## <span id="Automation_Engine_Action1"></span>Automation Engine Action V

[Automation Engine Action H](Automation_Engine_Action_H)

<div class="use">

Use this page to [Modify Actions](../Use_Cases/Modify_Actions).

</div>

Field

Description

Action Settings

Action

Displays the Action in a DSP® component that calls the AE Task or Task
Group stored in the AEID.  This field is not editable and the value is
set by the software developers. It aligns with a specific event in one
or many modules.

AEID

Displays the AE Task or Task Group that is executed when the event
specified by the Action is executed.  By changing this value, the action
that runs for an event in a module can be modified.

Execution Settings

Execution ID

Displays an ID that uniquely identifies an execution of the AEID.  If
set, this value is passed through to the Automation Engine History table
and uniquely identifies the execution of the AE.

Target Data Source ID

Displays the Data Source ID against which the AEID is executed.

Form Statement Only

If enabled, the Instruction text is formed and logged, but not executed.

Continue On Error

If enabled, when the Automation Engine is executing the AEID, and a
failure or error occurs, the processing of the AEID proceeds.
