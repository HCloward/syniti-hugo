+++
title = 'Content WebApp Examples'
solution = 'Data Quality'
+++

# Content WebApp Examples

The following examples can be used as reference when creating the
Content WebApp.

  - [Examples for dspConduct™ to Call boa (Add/Edit/Delete)
    Functions](#Content_WebApp_Examples_for_dspConduct_to_Call_boa_Add_Edit_Delete_Functions)
  - [Security Views for Binding Security by OrgUnits and Security that
    is not
    Bounded](#Security_Views_for_Binding_Security_by_OrgUnits_and_Security_that_is_not_Bounded_by_any_OrgUnits)
  - [Role Status BY User
Views](#Role_Status_BY_User_Views)

## <span id="Content_WebApp_Examples_for_dspConduct_to_Call_boa_Add_Edit_Delete_Functions"></span>Examples for dspConduct™ to Call boa (Add/Edit/Delete) Functions

The bit flag “Exists” must always have a 0 or 1 value and depicts if the
data already exists in the system(s) of record.

In the examples below, “ControlView” refers to any control view that the
WebApp Designer wants to use. These are commonly the Data or Page
Control Views that can be generated from the *[Scenario Role Task
Page](../Page_Desc/Scenario_Role_Task_Page.htm)* in dspConduct™.  Refer
to [Create Tables and Views for Content WebApp Pages
Overview](Create_Tables_and_Views_for_Content_WebApp_Pages_Overview.htm)
for more information.

 

<span>DGE.dbo.apiSecurityScenarioEdit(\[PageTable\].Exists,
ControlView.ScenarioID) \* DGE.dbo.apiRoleEdit(ControlView.RoleID,
ControlView.TaskID)</span>

<span>as boaEdit</span>

 

<span>DGE.dbo.apiSecurityScenarioDel(PageTable.Exists) \*
ISNULL(DGE.dbo.apiRoleEdit(ControlView.RoleID, ControlView.TaskID),
0)</span>

<span>as boaDel</span>

 

<span>ISNULL(DGE.dbo.apiSecurityScenarioEdit(pt.Exists,
dbo.ttRequest.ScenarioID), 0) \* ISNULL(DGE.dbo.apiRoleEdit(dcv.RoleID,
dcv.TaskID), 0) AS
boaAdd</span>

## <span id="Security_Views_for_Binding_Security_by_OrgUnits_and_Security_that_is_not_Bounded_by_any_OrgUnits"></span>Security Views for Binding Security by OrgUnits and Security that is not Bounded by any OrgUnits

**NOTE**: This view must be created prior to [creating the Role Status
BY User Views](#Role_Status_BY_User_Views).

 

<span style="font-family: &#39;Arial Narrow&#39;, sans-serif;">USE
\[DGE\]</span>

<span style="font-family: &#39;Arial Narrow&#39;, sans-serif;">GO</span>

 

<span style="font-family: &#39;Arial Narrow&#39;, sans-serif;">/\*\*\*\*\*\*
Object:<span> </span> Table
\[dbo\].\[ttSecurityCacheOrgUnit2\]<span>   </span> Script Date:
4/22/2016 9:06:07 AM \*\*\*\*\*\*/</span>

<span style="font-family: &#39;Arial Narrow&#39;, sans-serif;">SET
ANSI\_NULLS ON</span>

<span style="font-family: &#39;Arial Narrow&#39;, sans-serif;">GO</span>

 

<span style="font-family: &#39;Arial Narrow&#39;, sans-serif;">SET
QUOTED\_IDENTIFIER ON</span>

<span style="font-family: &#39;Arial Narrow&#39;, sans-serif;">GO</span>

 

<span style="font-family: &#39;Arial Narrow&#39;, sans-serif;">IF NOT
EXISTS (SELECT \* FROM sys.objects WHERE object\_id =
OBJECT\_ID(N'\[dbo\].\[ttSecurityCacheOrgUnit2\]') AND type in
(N'U'))</span>

<span style="font-family: &#39;Arial Narrow&#39;, sans-serif;">BEGIN</span>

<span style="font-family: &#39;Arial Narrow&#39;, sans-serif;">CREATE
TABLE
\[dbo\].\[ttSecurityCacheOrgUnit2\](</span>

<span style="font-family: &#39;Arial Narrow&#39;, sans-serif;"><span>             </span> \[UserID\]
\[nvarchar\](50) NOT
NULL,</span>

<span style="font-family: &#39;Arial Narrow&#39;, sans-serif;"><span>             </span> \[RoleID\]
\[uniqueidentifier\] NOT
NULL,</span>

<span style="font-family: &#39;Arial Narrow&#39;, sans-serif;"><span>             </span> \[OrgUnitValue\]
\[nvarchar\](50) NOT
NULL,</span>

<span style="font-family: &#39;Arial Narrow&#39;, sans-serif;"><span>             </span> \[ReadOnly\]
\[bit\] NOT
NULL,</span>

<span style="font-family: &#39;Arial Narrow&#39;, sans-serif;"><span> </span>CONSTRAINT
\[PK\_ttSecurityCacheOrgUnit2\] PRIMARY KEY
CLUSTERED</span>

<span style="font-family: &#39;Arial Narrow&#39;, sans-serif;">(</span>

<span style="font-family: &#39;Arial Narrow&#39;, sans-serif;"><span>             </span> \[RoleID\]
ASC,</span>

<span style="font-family: &#39;Arial Narrow&#39;, sans-serif;"><span>             </span> \[UserID\]
ASC,</span>

<span style="font-family: &#39;Arial Narrow&#39;, sans-serif;"><span>             </span> \[OrgUnitValue\]
ASC</span>

<span style="font-family: &#39;Arial Narrow&#39;, sans-serif;">)WITH
(PAD\_INDEX = OFF, STATISTICS\_NORECOMPUTE = OFF, IGNORE\_DUP\_KEY =
OFF, ALLOW\_ROW\_LOCKS = ON, ALLOW\_PAGE\_LOCKS = ON, FILLFACTOR =
80)</span>

<span style="font-family: &#39;Arial Narrow&#39;, sans-serif;">)</span>

<span style="font-family: &#39;Arial Narrow&#39;, sans-serif;">END</span>

<span style="font-family: &#39;Arial Narrow&#39;, sans-serif;">GO</span>

 

<span style="font-family: &#39;Arial Narrow&#39;, sans-serif;">/\*\*\*\*\*\*
Object:<span> </span> Table
\[dbo\].\[ttSecurityCacheOrgUnit3\]<span>   </span> Script Date:
4/22/2016 9:06:07 AM \*\*\*\*\*\*/</span>

<span style="font-family: &#39;Arial Narrow&#39;, sans-serif;">SET
ANSI\_NULLS ON</span>

<span style="font-family: &#39;Arial Narrow&#39;, sans-serif;">GO</span>

 

<span style="font-family: &#39;Arial Narrow&#39;, sans-serif;">SET
QUOTED\_IDENTIFIER ON</span>

<span style="font-family: &#39;Arial Narrow&#39;, sans-serif;">GO</span>

 

<span style="font-family: &#39;Arial Narrow&#39;, sans-serif;">IF NOT
EXISTS (SELECT \* FROM sys.objects WHERE object\_id =
OBJECT\_ID(N'\[dbo\].\[ttSecurityCacheOrgUnit3\]') AND type in
(N'U'))</span>

<span style="font-family: &#39;Arial Narrow&#39;, sans-serif;">BEGIN</span>

<span style="font-family: &#39;Arial Narrow&#39;, sans-serif;">CREATE
TABLE
\[dbo\].\[ttSecurityCacheOrgUnit3\](</span>

<span style="font-family: &#39;Arial Narrow&#39;, sans-serif;"><span>             </span> \[UserID\]
\[nvarchar\](50) NOT
NULL,</span>

<span style="font-family: &#39;Arial Narrow&#39;, sans-serif;"><span>             </span> \[RoleID\]
\[uniqueidentifier\] NOT
NULL,</span>

<span style="font-family: &#39;Arial Narrow&#39;, sans-serif;"><span>             </span> \[OrgUnitValue\]
\[nvarchar\](50) NOT
NULL,</span>

<span style="font-family: &#39;Arial Narrow&#39;, sans-serif;"><span>             </span> \[ReadOnly\]
\[bit\] NOT
NULL,</span>

<span style="font-family: &#39;Arial Narrow&#39;, sans-serif;"><span> </span>CONSTRAINT
\[PK\_ttSecurityCacheOrgUnit3\] PRIMARY KEY
CLUSTERED</span>

<span style="font-family: &#39;Arial Narrow&#39;, sans-serif;">(</span>

<span style="font-family: &#39;Arial Narrow&#39;, sans-serif;"><span>             </span> \[RoleID\]
ASC,</span>

<span style="font-family: &#39;Arial Narrow&#39;, sans-serif;"><span>             </span> \[UserID\]
ASC,</span>

<span style="font-family: &#39;Arial Narrow&#39;, sans-serif;"><span>             </span> \[OrgUnitValue\]
ASC</span>

<span style="font-family: &#39;Arial Narrow&#39;, sans-serif;">)WITH
(PAD\_INDEX = OFF, STATISTICS\_NORECOMPUTE = OFF, IGNORE\_DUP\_KEY =
OFF, ALLOW\_ROW\_LOCKS = ON, ALLOW\_PAGE\_LOCKS = ON, FILLFACTOR =
80)</span>

<span style="font-family: &#39;Arial Narrow&#39;, sans-serif;">)</span>

<span style="font-family: &#39;Arial Narrow&#39;, sans-serif;">END</span>

<span style="font-family: &#39;Arial Narrow&#39;, sans-serif;">GO</span>

 

<span style="font-family: &#39;Arial Narrow&#39;, sans-serif;">/\*\*\*\*\*\*
Object:<span> </span> Table
\[dbo\].\[ttSecurityCacheOrgUnit1\]<span>   </span> Script Date:
4/22/2016 9:06:07 AM \*\*\*\*\*\*/</span>

<span style="font-family: &#39;Arial Narrow&#39;, sans-serif;">SET
ANSI\_NULLS ON</span>

<span style="font-family: &#39;Arial Narrow&#39;, sans-serif;">GO</span>

 

<span style="font-family: &#39;Arial Narrow&#39;, sans-serif;">SET
QUOTED\_IDENTIFIER ON</span>

<span style="font-family: &#39;Arial Narrow&#39;, sans-serif;">GO</span>

 

<span style="font-family: &#39;Arial Narrow&#39;, sans-serif;">IF NOT
EXISTS (SELECT \* FROM sys.objects WHERE object\_id =
OBJECT\_ID(N'\[dbo\].\[ttSecurityCacheOrgUnit1\]') AND type in
(N'U'))</span>

<span style="font-family: &#39;Arial Narrow&#39;, sans-serif;">BEGIN</span>

<span style="font-family: &#39;Arial Narrow&#39;, sans-serif;">CREATE
TABLE
\[dbo\].\[ttSecurityCacheOrgUnit1\](</span>

<span style="font-family: &#39;Arial Narrow&#39;, sans-serif;"><span>             </span> \[UserID\]
\[nvarchar\](50) NOT
NULL,</span>

<span style="font-family: &#39;Arial Narrow&#39;, sans-serif;"><span>             </span> \[RoleID\]
\[uniqueidentifier\] NOT
NULL,</span>

<span style="font-family: &#39;Arial Narrow&#39;, sans-serif;"><span>             </span> \[OrgUnitValue\]
\[nvarchar\](50) NOT
NULL,</span>

<span style="font-family: &#39;Arial Narrow&#39;, sans-serif;"><span>             </span> \[ReadOnly\]
\[bit\] NOT NULL DEFAULT
((0)),</span>

<span style="font-family: &#39;Arial Narrow&#39;, sans-serif;"><span> </span>CONSTRAINT
\[PK\_ttSecurityCacheOrgUnit1\] PRIMARY KEY
CLUSTERED</span>

<span style="font-family: &#39;Arial Narrow&#39;, sans-serif;">(</span>

<span style="font-family: &#39;Arial Narrow&#39;, sans-serif;"><span>             </span> \[RoleID\]
ASC,</span>

<span style="font-family: &#39;Arial Narrow&#39;, sans-serif;"><span>             </span> \[UserID\]
ASC,</span>

<span style="font-family: &#39;Arial Narrow&#39;, sans-serif;"><span>             </span> \[OrgUnitValue\]
ASC</span>

<span style="font-family: &#39;Arial Narrow&#39;, sans-serif;">)WITH
(PAD\_INDEX = OFF, STATISTICS\_NORECOMPUTE = OFF, IGNORE\_DUP\_KEY =
OFF, ALLOW\_ROW\_LOCKS = ON, ALLOW\_PAGE\_LOCKS = ON, FILLFACTOR =
80)</span>

<span style="font-family: &#39;Arial Narrow&#39;, sans-serif;">)</span>

<span style="font-family: &#39;Arial Narrow&#39;, sans-serif;">END</span>

<span style="font-family: &#39;Arial Narrow&#39;, sans-serif;">GO</span>

 

<span style="font-family: &#39;Arial Narrow&#39;, sans-serif;">/\*NOTE:<span> </span> Replace
“dgeNameOfContentApp” below with the database name where these views
need to be created. There should be only one occurrence.\*/</span>

 

<span style="font-family: &#39;Arial Narrow&#39;, sans-serif;">USE
\[dgeNameOfContentApp\]</span>

<span style="font-family: &#39;Arial Narrow&#39;, sans-serif;">GO</span>

 

<span style="font-family: &#39;Arial Narrow&#39;, sans-serif;">/\*\*\*\*\*\*
Object:<span> </span> View
\[dbo\].\[ttSecurityCacheOrgUnit3\]<span>   </span> Script Date:
4/22/2016 9:06:07 AM \*\*\*\*\*\*/</span>

<span style="font-family: &#39;Arial Narrow&#39;, sans-serif;">SET
ANSI\_NULLS ON</span>

<span style="font-family: &#39;Arial Narrow&#39;, sans-serif;">GO</span>

 

<span style="font-family: &#39;Arial Narrow&#39;, sans-serif;">SET
QUOTED\_IDENTIFIER ON</span>

<span style="font-family: &#39;Arial Narrow&#39;, sans-serif;">GO</span>

 

<span style="font-family: &#39;Arial Narrow&#39;, sans-serif;">IF NOT
EXISTS (SELECT \* FROM sys.views WHERE object\_id =
OBJECT\_ID(N'\[dbo\].\[ttSecurityCacheOrgUnit3\]'))</span>

<span style="font-family: &#39;Arial Narrow&#39;, sans-serif;">EXEC
dbo.sp\_executesql @statement = N'</span>

 

<span style="font-family: &#39;Arial Narrow&#39;, sans-serif;">CREATE
VIEW
\[dbo\].\[ttSecurityCacheOrgUnit3\]</span>

<span style="font-family: &#39;Arial Narrow&#39;, sans-serif;">AS</span>

<span style="font-family: &#39;Arial Narrow&#39;, sans-serif;">SELECT<span>       </span> UserID,
RoleID, OrgUnitValue,
ReadOnly</span>

<span style="font-family: &#39;Arial Narrow&#39;, sans-serif;">FROM<span>           </span> DGE.dbo.ttSecurityCacheOrgUnit3</span>

 

 

<span style="font-family: &#39;Arial Narrow&#39;, sans-serif;">'</span>

<span style="font-family: &#39;Arial Narrow&#39;, sans-serif;">GO</span>

 

<span style="font-family: &#39;Arial Narrow&#39;, sans-serif;">/\*\*\*\*\*\*
Object:<span> </span> View
\[dbo\].\[ttSecurityCacheOrgUnit2\]<span>   </span> Script Date:
4/22/2016 9:06:07 AM \*\*\*\*\*\*/</span>

<span style="font-family: &#39;Arial Narrow&#39;, sans-serif;">SET
ANSI\_NULLS ON</span>

<span style="font-family: &#39;Arial Narrow&#39;, sans-serif;">GO</span>

 

<span style="font-family: &#39;Arial Narrow&#39;, sans-serif;">SET
QUOTED\_IDENTIFIER ON</span>

<span style="font-family: &#39;Arial Narrow&#39;, sans-serif;">GO</span>

 

<span style="font-family: &#39;Arial Narrow&#39;, sans-serif;">IF NOT
EXISTS (SELECT \* FROM sys.views WHERE object\_id =
OBJECT\_ID(N'\[dbo\].\[ttSecurityCacheOrgUnit2\]'))</span>

<span style="font-family: &#39;Arial Narrow&#39;, sans-serif;">EXEC
dbo.sp\_executesql @statement = N'</span>

<span style="font-family: &#39;Arial Narrow&#39;, sans-serif;">CREATE
VIEW
\[dbo\].\[ttSecurityCacheOrgUnit2\]</span>

<span style="font-family: &#39;Arial Narrow&#39;, sans-serif;">AS</span>

<span style="font-family: &#39;Arial Narrow&#39;, sans-serif;">SELECT<span>       </span> UserID,
RoleID, OrgUnitValue,
ReadOnly</span>

<span style="font-family: &#39;Arial Narrow&#39;, sans-serif;">FROM<span>        </span> <span>   </span>DGE.dbo.ttSecurityCacheOrgUnit2</span>

 

<span style="font-family: &#39;Arial Narrow&#39;, sans-serif;">'</span>

<span style="font-family: &#39;Arial Narrow&#39;, sans-serif;">GO</span>

 

<span style="font-family: &#39;Arial Narrow&#39;, sans-serif;">/\*\*\*\*\*\*
Object:<span> </span> View
\[dbo\].\[ttSecurityCacheOrgUnit1\]<span>   </span> Script Date:
4/22/2016 9:06:07 AM \*\*\*\*\*\*/</span>

<span style="font-family: &#39;Arial Narrow&#39;, sans-serif;">SET
ANSI\_NULLS ON</span>

<span style="font-family: &#39;Arial Narrow&#39;, sans-serif;">GO</span>

 

<span style="font-family: &#39;Arial Narrow&#39;, sans-serif;">SET
QUOTED\_IDENTIFIER ON</span>

<span style="font-family: &#39;Arial Narrow&#39;, sans-serif;">GO</span>

 

<span style="font-family: &#39;Arial Narrow&#39;, sans-serif;">IF NOT
EXISTS (SELECT \* FROM sys.views WHERE object\_id =
OBJECT\_ID(N'\[dbo\].\[ttSecurityCacheOrgUnit1\]'))</span>

<span style="font-family: &#39;Arial Narrow&#39;, sans-serif;">EXEC
dbo.sp\_executesql @statement = N'CREATE VIEW
\[dbo\].\[ttSecurityCacheOrgUnit1\]</span>

<span style="font-family: &#39;Arial Narrow&#39;, sans-serif;">AS</span>

<span style="font-family: &#39;Arial Narrow&#39;, sans-serif;">SELECT<span>       </span> UserID,
RoleID, OrgUnitValue,
ReadOnly</span>

<span style="font-family: &#39;Arial Narrow&#39;, sans-serif;">FROM<span>           </span> DGE.dbo.ttSecurityCacheOrgUnit1</span>

<span style="font-family: &#39;Arial Narrow&#39;, sans-serif;">'</span>

<span style="font-family: &#39;Arial Narrow&#39;, sans-serif;">GO</span>

 

<span style="font-family: &#39;Arial Narrow&#39;, sans-serif;">USE
\[DGE\]</span>

<span style="font-family: &#39;Arial Narrow&#39;, sans-serif;">GO</span>

 

<span style="font-family: &#39;Arial Narrow&#39;, sans-serif;">IF NOT
EXISTS (SELECT \* FROM dbo.sysobjects WHERE id =
OBJECT\_ID(N'\[dbo\].\[DF\_\_ttSecurit\_\_ReadO\_\_0EF1425F\]') AND type
=
'D')</span>

<span style="font-family: &#39;Arial Narrow&#39;, sans-serif;">BEGIN</span>

<span style="font-family: &#39;Arial Narrow&#39;, sans-serif;">ALTER
TABLE \[dbo\].\[ttSecurityCacheOrgUnit2\] ADD<span> </span> DEFAULT
((0)) FOR
\[ReadOnly\]</span>

<span style="font-family: &#39;Arial Narrow&#39;, sans-serif;">END</span>

 

<span style="font-family: &#39;Arial Narrow&#39;, sans-serif;">GO</span>

 

<span style="font-family: &#39;Arial Narrow&#39;, sans-serif;">IF NOT
EXISTS (SELECT \* FROM dbo.sysobjects WHERE id =
OBJECT\_ID(N'\[dbo\].\[DF\_\_ttSecurit\_\_ReadO\_\_0FE56698\]') AND type
=
'D')</span>

<span style="font-family: &#39;Arial Narrow&#39;, sans-serif;">BEGIN</span>

<span style="font-family: &#39;Arial Narrow&#39;, sans-serif;">ALTER
TABLE \[dbo\].\[ttSecurityCacheOrgUnit3\] ADD<span> </span> DEFAULT
((0)) FOR
\[ReadOnly\]</span>

<span style="font-family: &#39;Arial Narrow&#39;, sans-serif;">END</span>

 

<span style="font-family: &#39;Arial Narrow&#39;, sans-serif;">GO</span>

 

<span>CREATE VIEW \[dbo\].\[webSecurity\_UnboundedSel\]</span>

<span>AS</span>

<span>SELECT        RequestID, RoleID, UserID AS boaUserID,
ReadOnly</span>

<span>FROM            dbo.ttRequestRoleUser</span>

 

<span>GO</span>

 

 

<span>CREATE VIEW \[dbo\].\[webSecurity\_BoundByOrgUnit1Sel\]</span>

<span>AS</span>

<span>SELECT        dbo.ttRequestRoleUser.RequestID,
dbo.ttSecurityCacheOrgUnit1.RoleID,
dbo.ttSecurityCacheOrgUnit1.OrgUnitValue AS OrgUnit1,
dbo.ttSecurityCacheOrgUnit1.UserID AS
boaUserID,</span>

<span>                         dbo.ttSecurityCacheOrgUnit1.ReadOnly</span>

<span>FROM            dbo.ttSecurityCacheOrgUnit1 INNER JOIN</span>

<span>                         dbo.ttRequestRoleUser ON
dbo.ttSecurityCacheOrgUnit1.RoleID = dbo.ttRequestRoleUser.RoleID AND
dbo.ttSecurityCacheOrgUnit1.UserID = dbo.ttRequestRoleUser.UserID</span>

 

<span>GO</span>

 

<span>/\*\*\*\*\*\* Object:  View
\[dbo\].\[webSecurity\_BoundByOrgUnit2Sel\]    Script Date: 3/1/2016
10:39:11 PM \*\*\*\*\*\*/</span>

<span>SET ANSI\_NULLS ON</span>

<span>GO</span>

 

<span>SET QUOTED\_IDENTIFIER ON</span>

<span>GO</span>

 

<span>CREATE VIEW \[dbo\].\[webSecurity\_BoundByOrgUnit2Sel\]</span>

<span>AS</span>

<span>SELECT        dbo.ttRequestRoleUser.RequestID,
dbo.ttSecurityCacheOrgUnit2.RoleID,
dbo.ttSecurityCacheOrgUnit2.OrgUnitValue AS OrgUnit2,
dbo.ttSecurityCacheOrgUnit2.UserID AS
boaUserID,</span>

<span>                         dbo.ttSecurityCacheOrgUnit2.ReadOnly</span>

<span>FROM            dbo.ttSecurityCacheOrgUnit2 INNER JOIN</span>

<span>                         dbo.ttRequestRoleUser ON
dbo.ttSecurityCacheOrgUnit2.RoleID = dbo.ttRequestRoleUser.RoleID AND
dbo.ttSecurityCacheOrgUnit2.UserID = dbo.ttRequestRoleUser.UserID</span>

 

<span>GO</span>

 

<span>/\*\*\*\*\*\* Object:  View
\[dbo\].\[webSecurity\_BoundByOrgUnit3Sel\]    Script Date: 3/1/2016
10:39:11 PM \*\*\*\*\*\*/</span>

<span>SET ANSI\_NULLS ON</span>

<span>GO</span>

 

<span>SET QUOTED\_IDENTIFIER ON</span>

<span>GO</span>

 

<span>CREATE VIEW \[dbo\].\[webSecurity\_BoundByOrgUnit3Sel\]</span>

<span>AS</span>

<span>SELECT        dbo.ttRequestRoleUser.RequestID,
dbo.ttSecurityCacheOrgUnit3.RoleID,
dbo.ttSecurityCacheOrgUnit3.OrgUnitValue AS OrgUnit3,
dbo.ttSecurityCacheOrgUnit3.UserID AS
boaUserID,</span>

<span>                         dbo.ttSecurityCacheOrgUnit3.ReadOnly</span>

<span>FROM            dbo.ttSecurityCacheOrgUnit3 INNER JOIN</span>

<span>                         dbo.ttRequestRoleUser ON
dbo.ttSecurityCacheOrgUnit3.UserID = dbo.ttRequestRoleUser.UserID AND
dbo.ttSecurityCacheOrgUnit3.RoleID = dbo.ttRequestRoleUser.RoleID</span>

 

<span>GO</span>

<span style="font-family: &#39;Arial Narrow&#39;, sans-serif;">/\*A
Content Request page may need ScenarioID to be set on the *Vertical*
View to drive configuration for scenario-based field controls on the
Request page.<span> </span> In this case, the Request page must have an
INSERT MODE of “Horizontal Insert/Switch To Vertical” and the following
Trigger that calls the above-suggested OnValidate procedure at the
trigger level.\*/</span>

 

<span>CREATE TRIGGER \[dbo\].\[trgRequest\_BusinessProcessScenarioIns\]
ON \[dbo\].\[ttRequest\] </span>

<span>FOR INSERT </span>

<span>AS </span>

<span>DECLARE @BusinessProcessID uniqueidentifier </span>

<span>DECLARE @ScenarioID uniqueidentifier</span>

<span>DECLARE @ContentRequestID uniqueidentifier</span>

<span>DECLARE @RequestID int </span>

<span>DECLARE @boaUserID nvarchar(50)</span>

<span>IF UPDATE (ScenarioID) </span>

<span>BEGIN </span>

<span>SET @ScenarioID = ISNULL((SELECT ScenarioID FROM INSERTED),
NULL) </span>

<span>SET @ContentRequestID = (SELECT ContentRequestID FROM
INSERTED)</span>

<span>SET @boaUserID = (SELECT AddedBy FROM INSERTED) </span>

<span>IF (@ScenarioID IS NULL) </span>

<span>BEGIN </span>

<span>SET @BusinessProcessID = (SELECT BusinessProcessID FROM ttRequest
WHERE</span><span>ContentRequestID
=</span><span>@ContentRequestID) </span>

 

<span>EXEC webRequest\_OnValidate\_CreateRequest @ContentRequestID,
@BusinessProcessID, @boaUserID</span>

<span>END</span>

<span>END</span>

## <span id="Role_Status_BY_User_Views"></span>Role Status BY User Views

<span style="font-weight: bold;">NOTE</span>: The [Unbounded Security
view](Content_WebApp_Examples.htm#Security_Views_for_Binding_Security_by_OrgUnits_and_Security_that_is_not_Bounded_by_any_OrgUnits)
must be created prior to creating these views.

 

<span>/\*\*\*\*\*\* Object:  View
\[dbo\].\[webRequest\_RoleStatusByUser0Sel\]    Script Date: 3/2/2016
10:47:00 PM \*\*\*\*\*\*/</span>

<span>SET ANSI\_NULLS ON</span>

<span>GO</span>

 

<span>SET QUOTED\_IDENTIFIER ON</span>

<span>GO</span>

 

 

<span>CREATE VIEW \[dbo\].\[webRequest\_RoleStatusByUser0Sel\]</span>

<span>AS</span>

<span>SELECT        dbo.ttRequest.RequestID, dbo.ttRequestRole.RoleID,
dbo.ttRequestRoleSLA.DueDate, dbo.ttRequestRoleSLA.LastEvaluation</span>

<span>FROM            dbo.ttRequest INNER JOIN</span>

<span>                         dbo.ttRequestRole ON
dbo.ttRequest.RequestID = dbo.ttRequestRole.RequestID INNER JOIN</span>

<span>                         dbo.ttRequestRoleSLA ON
dbo.ttRequestRole.RequestID = dbo.ttRequestRoleSLA.RequestID AND
dbo.ttRequestRole.RoleID = dbo.ttRequestRoleSLA.RoleID</span>

<span>WHERE        (dbo.ttRequestRole.DependencyComplete = 1) AND
(dbo.ttRequestRole.Finished = 0)</span>

 

 

<span>GO</span>

 

<span>/\*\*\*\*\*\* Object:  View
\[dbo\].\[webRequest\_RoleStatusByUser1Sel\]    Script Date: 3/2/2016
10:47:00 PM \*\*\*\*\*\*/</span>

<span>SET ANSI\_NULLS ON</span>

<span>GO</span>

 

<span>SET QUOTED\_IDENTIFIER ON</span>

<span>GO</span>

 

 

<span>CREATE VIEW \[dbo\].\[webRequest\_RoleStatusByUser1Sel\]</span>

<span>AS</span>

<span>SELECT        dbo.webSecurity\_UnboundedSel.RequestID,
dbo.webSecurity\_UnboundedSel.RoleID,
dbo.webSecurity\_UnboundedSel.boaUserID, CASE WHEN SubmittedOn IS
NULL </span>

<span>                         THEN '0' WHEN Finished = '1' THEN '1'
WHEN Finished = '0' AND DependencyComplete = '0' THEN '2' WHEN Finished
= '0' AND DependencyComplete = '1' AND </span>

<span>                         NOT COALESCE
(webRequest\_RoleStatusByUser0Sel.DueDate, GETDATE()) \< GETDATE() THEN
'3' WHEN Finished = '0' AND DependencyComplete = '1' AND </span>

<span>                         webRequest\_RoleStatusByUser0Sel.DueDate
\< GETDATE() THEN '4' END AS RoleStatus</span>

<span>FROM            dbo.webSecurity\_UnboundedSel INNER JOIN</span>

<span>                         dbo.ttRequestRole ON
dbo.webSecurity\_UnboundedSel.RequestID = dbo.ttRequestRole.RequestID
AND dbo.webSecurity\_UnboundedSel.RoleID = dbo.ttRequestRole.RoleID
INNER JOIN</span>

<span>                         dbo.ttRequest ON
dbo.ttRequestRole.RequestID = dbo.ttRequest.RequestID LEFT OUTER
JOIN</span>

<span>                         dbo.webRequest\_RoleStatusByUser0Sel ON
dbo.ttRequestRole.RequestID =
dbo.webRequest\_RoleStatusByUser0Sel.RequestID AND
dbo.ttRequestRole.RoleID =
dbo.webRequest\_RoleStatusByUser0Sel.RoleID</span>

 

 

<span>GO</span>

 

<span>/\*\*\*\*\*\* Object:  View
\[dbo\].\[webRequest\_RoleStatusByUser2Sel\]    Script Date: 3/2/2016
10:47:00 PM \*\*\*\*\*\*/</span>

<span>SET ANSI\_NULLS ON</span>

<span>GO</span>

 

<span>SET QUOTED\_IDENTIFIER ON</span>

<span>GO</span>

 

 

<span>CREATE VIEW \[dbo\].\[webRequest\_RoleStatusByUser2Sel\]</span>

<span>AS</span>

<span>SELECT        RequestID, boaUserID, MAX(CAST(RoleStatus AS int))
AS RoleStatus</span>

<span>FROM            dbo.webRequest\_RoleStatusByUser1Sel</span>

<span>GROUP BY RequestID, boaUserID</span>

 

 

<span>GO</span>

 

<span>/\*\*\*\*\*\* Object:  View
\[dbo\].\[webRequest\_RoleStatusByUser3Sel\]    Script Date: 3/2/2016
10:47:00 PM \*\*\*\*\*\*/</span>

<span>SET ANSI\_NULLS ON</span>

<span>GO</span>

 

<span>SET QUOTED\_IDENTIFIER ON</span>

<span>GO</span>

 

 

<span>CREATE VIEW \[dbo\].\[webRequest\_RoleStatusByUser3Sel\]</span>

<span>AS</span>

<span>SELECT        RequestID, boaUserID, CASE WHEN RoleStatus = '1'
THEN 'BlueCheck' WHEN RoleStatus = '3' THEN 'GreenPlus' WHEN RoleStatus
= '4' THEN 'RedX' ELSE 'YellowYieldWithExclamation' END AS RS</span>

<span>FROM            dbo.webRequest\_RoleStatusByUser2Sel</span>

 

 

<span data-xmlns="http://www.w3.org/1999/xhtml">GO</span>
