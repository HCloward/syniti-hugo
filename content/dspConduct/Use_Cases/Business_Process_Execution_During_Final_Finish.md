+++
title = 'Business Process Execution During Final Finish'
solution = 'Data Quality'
+++

# Business Process Execution During Final Finish

If the scenarios in a business process do not have scenario
dependencies, the priority order of the scenarios determine the order
that data is posted to a target system for the request.

If scenario dependencies exist, the child scenario is processed when its
dependent scenario is complete. Refer to [Business Process Execution
with Scenario Dependencies During Final
Finish](Business_Process_Execution_with_Scenario_Dependencies_During_Final_Finish.htm)
for more information.

<span style="font-weight: bold;">NOTE</span>: For new requests that are
automatically created as part of a multi-scenario business process, the
Content Request page OnValidate event is automatically executed. The
Cransoft UserID 'process' must have access to the Content Request page
in order to execute the OnValidate event.

For example, a business process has 4 scenarios:

1.  Create FinishedGood Make – Reservation” has priority 10, no child
    scenario criteria.<span> </span>Original parent request has 3
    distinct values for OrgUnit1 and 3 distinct values for OrgUnit2.
2.  Extend FinishedGood Make – Mfg”<span> </span> has priority 20, child
    scenario criteria = “Plant” (OrgUnit1)
3.  Extend FinishedGood Make – Sls” has priority 20, child scenario
    criteria = “SalesOrg” (OrgUnit2)
4.  Change Basic Data – Activate” has priority 40 , no child scenario
    criteria

In the following example, a business process is designed to reserve a
Material Number in SAP. When the Material Master is created/posted, it
is automatically placed on hold status in SAP. dspConduct™ invokes the
next scenario in the business process based on the priority order.

The reserved material is extended to multiple Plants (OrgUnit1) and
Sales Organizations (OrgUnit2) based on the values assigned to the
parent request. dspConduct™ automatically invokes the last scenario when
all child requests are posted to SAP and the posting roles are finished.
The material is then taken off hold status and is made available for
general use (with the scenario with priority 40, ”Change Basic
Data-Activate” below).

The following is an example of the requests that are created as a result
of the business process definition previously stated and the values
entered into the parent request.

**NOTE:** Valid Values are **OrgUnit1**, **OrgUnit2** or
**OrgUnit3**.<span>  </span>

Priority

Scenario

OrgUnit1

OrgUnit2

OrgUnit3

Child Scenario Criteria

Request

10

Create FinishedGood Make - Reservation

0001

1000

2000

0001

BOA1

BOA2

BOA

CranSoft

Blank

Parent

After the parent request is posted to SAP, dspConduct™ creates the
following 6 child requests.

20

Extend FinishedGood Make - Mfg

0001

0001

BOA1

BOA2

BOA

CranSoft

OrgUnit1

Child – 1

20

Extend FinishedGood Make - Mfg

1000

0001

BOA1

BOA2

BOA

CranSoft

OrgUnit1

Child – 2

20

Extend FinishedGood Make - Mfg

2000

0001

BOA1

BOA2

BOA

CranSoft

OrgUnit1

Child – 3

20

Extend FinishedGood Make - Sls

0001

1000

2000

0001

BOA

CranSoft

OrgUnit2

Child – 4

20

Extend FinishedGood Make - Sls

0001

1000

2000

BOA1

BOA

CranSoft

OrgUnit2

Child – 5

20

Extend FinishedGood Make - Sls

0001

1000

2000

BOA2

BOA

CranSoft

OrgUnit2

Child – 6

After all 6 child requests are posted to SAP, dspConduct™ creates the
following child request.

40

Change Basic Data-Activate

0001

1000

2000

0001

BOA1

BOA2

BOA

CranSoft

Blank

Child – 7
