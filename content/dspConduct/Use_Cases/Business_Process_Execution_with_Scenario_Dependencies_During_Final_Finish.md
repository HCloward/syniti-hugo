+++
title = 'Business Process Execution with Scenario Dependencies During Final Finish'
solution = 'Data Quality'
+++

# Business Process Execution with Scenario Dependencies During Final Finish

When a request is finished, if the business process has scenario
dependencies, those dependencies determine the order that data is posted
to a target system for the request.

If a scenario dependency exists, the child scenario is processed when
its dependent scenario is complete.

If no scenario dependencies are present, requests are created and posted
based on scenario priority. Refer to [Business Process Execution During
Final Finish](Business_Process_Execution_During_Final_Finish.htm) for
more information.

For example, business process 1 has scenarios A and D. At the scenario
level, scenario D is dependent on scenario A, B and C. For business
process 1, scenario D is dependent on scenario A because scenarios B and
C are not part of business process 1. In business process 2, scenarios
A, B, C and D are configured. Scenario D is dependent on scenario A, B
and C being completed before D as all three are relevant to scenario D’s
business process.

**NOTE**: Dependencies are considered completed even when a scenario
exists as a dependency but is not technically part of the business
process. In the example of business process 1 above, scenarios B and C
are complete, even though they are not included in the business process.

<span style="font-weight: bold;">NOTE</span>: A dependent scenario may
exist in another category. Refer to [Allow a Scenario to be used in
Other Categories](Allow_a_Scenario_to_be_used_in_Other_Categories.htm)
for more information.

<span style="font-weight: bold;">NOTE</span>: When a business process
uses a scenario from another category, the request that is created for
that scenario will be created in the database/Webapp that is the default
WebApp for that other category. For example, a category called Northwest
Region has a default WebApp of NWRegion. It  contains a scenario called
Create SoldTo – General Data. This scenario has been configured for use
in the category US Operations. A scenario in US Operations is Create
SoldTo. A user could create a business process in the US Operations
category that uses the Create SoldTo scenario as a parent of the Create
SoldTo – General Data scenario from the Northwest Region category. When
the business process is executed, a request is created in the NWRegion
WebApp.  

<span style="font-weight: bold;">NOTE</span>: For new requests that are
automatically created as part of a multi-scenario business process, the
Content Request page OnValidate event is automatically executed. The
Cransoft UserID 'process' must have access to the Content Request page
in order to execute the OnValidate event.

Refer to [Assign a Dependent Scenario to a
Scenario](Add_a_Dependent_Scenario.htm) for more information.

For example, a business process has 4 scenarios:

1.  Create FinishedGood Make – Reservation” has priority 10, no child
    scenario criteria.<span> </span>Original parent request has 3
    distinct values for OrgUnit1 and 3 distinct values for OrgUnit2.
2.  Extend FinishedGood Make – Mfg”<span> </span> has priority 20, child
    scenario criteria = “Plant” (OrgUnit1). This scenario does not have
    a dependency relationship.
3.  Extend FinishedGood Make – Sls” has priority 30, child scenario
    criteria = “SalesOrg” (OrgUnit2).This scenario is dependent on the
    scenario “Create FinishedGood Make – Reservation."
4.  Change Basic Data – Activate” has priority 40 , no child scenario
    criteria

In the following example, a business process is designed to reserve a
Material Number in SAP. When the Material Master is created/posted, it
is automatically placed on hold status in SAP. dspConduct™ invokes the
next scenario in the business process based on the scenario dependency.
Once that dependency is complete, the scenario with the next highest
priority is executed.

The reserved material is extended to Sales Organizations (OrgUnit2)
prior to being extended to multiple Plants (OrgUnit1) based on the
values assigned to the parent request. dspConduct™ automatically invokes
the last scenario when all child requests are posted to SAP and the
posting roles are finished. The material is then taken off hold status
and is made available for general use<span> </span> (with the scenario
with priority 40, ”Change Basic Data-Activate” below).

The following is an example of the order the requests are created as a
result of the business process definition previously stated and the
values entered into the parent request.

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

30

Extend FinishedGood Make - Sls

0001

1000

2000

0001

BOA

CranSoft

OrgUnit2

Child – 1

30

Extend FinishedGood Make - Sls

0001

1000

2000

BOA1

BOA

CranSoft

OrgUnit2

Child – 2

30

Extend FinishedGood Make - Sls

0001

1000

2000

BOA2

BOA

CranSoft

OrgUnit2

Child – 3

20

Extend FinishedGood Make - Mfg

0001

0001

BOA1

BOA2

BOA

CranSoft

OrgUnit1

Child – 4

20

Extend FinishedGood Make - Mfg

1000

0001

BOA1

BOA2

BOA

CranSoft

OrgUnit1

Child – 5

20

Extend FinishedGood Make - Mfg

2000

0001

BOA1

BOA2

BOA

CranSoft

OrgUnit1

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
