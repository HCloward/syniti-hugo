# Naming Conventions and the Enforce Strict Naming Feature

The DSP® is delivered with a BOA pre-defined naming convention for
Stored Procedures and *Horizontal*, *Vertical*, Validation and Control
Views, to name a few. The defined naming conventions can be set at the
platform level on the *Vertical* View of the
*[Parameters](../Sys_Admin/Page_Desc/Parameters_All_TabsSysAdmin.htm#Naming_Conventions_Tab)*
page on the Naming Conventions tab. These values are the default values
for WebApps, but can be updated at the WebApp level on the *Vertical*
View of the *[WebApps](../Sys_Admin/Page_Desc/WebApps_H.htm)* page.
Naming conventions entered at the WebApp level override those set at the
platform level.

**NOTE**: Views in the underlying database must be named with the
associated table name from the page registration.

Naming Conventions simplify list box options in DSP® by limiting the
objects associated with any given page.

At the WebApp level, if the Enforce Strict Naming checkbox is enabled on
the Naming Options tab on the *Vertical* View of the
*[WebApps](../Sys_Admin/Page_Desc/WebApps_H.htm)* page, the DSP® filters
applicable list boxes based on the naming conventions. For example, a
WebApp has a page using the nwEmployee table. With Enforce Strict Naming
enabled, all views registered to this page must contain the word
Employee within the name of the view and with the proper naming
convention prefix and suffix. For a Horizontal View, web is the prefix
and Hor is the suffix. For a Vertical page, web is the prefix and Ver is
the suffix.

|                    |                              |
| ------------------ | ---------------------------- |
| Correct            | Incorrect (Will not display) |
| webEmployeeHor     | Employee                     |
| webEmployeeHor     | EmployeeHor                  |
| webEmployeeVer     | webWorkerVer                 |
| webEmployeeTypeHor | webTypeHor                   |

The default **Table Prefix Size** is **2** for the WebApp and indicates
the first two characters (prefix) are for registration purposes and are
not included as part of the table name for consideration with Enforce
Strict Naming. For example, the tables in **Northwind** are prefixed
with **nw**, **xt** or **zt**. The **nw** is ignored when filtering any
views based for a page where the **nwEmployee** table is registered.

If, when selecting a view from a list box, the needed view is not
available, check the Naming Conventions tab for the active WebApp and
compare it to the table and view names for that page.
