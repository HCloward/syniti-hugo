+++
title = "DSP App Dev Overview"
weight = 3
layout = "single"
solution = "Platform"
+++

# DSP® Application Development Overview

The Data Stewardship Platform (DSP®) architecture creates powerfully
simple, codeless web applications, known as WebApps, with inherent
business logic. The platform offers a robust way to dynamically design
scalable and secure WebApps that complement or extend business
processes.

The DSP® is the framework upon which all WebApps, including itself, are
built. Though the architecture is similar to that of nearly every other
web-based product, DSP® pages are never created with interpreted or
compiled code from files stored on the web server. The engine directly
renders WebApp pages in the client browser based on metadata stored
within DSP®. All the information used to create the functionality and
controls of an application is stored as dynamically updateable data, not
as code, and the content seen in a client web browser is generated on
the fly in the browser itself.

**NOTE:  <span style="font-weight: normal;">It is assumed that the
audience has a working knowledge of SQL, including creating tables, and
creating and optimizing views and stored procedures. The performance of
a WebApp as measured by the responsiveness of the web pages and the
overall user experience is directly affected by, and very sensitive to,
the performance of the views and stored procedures created for the
WebApp by the DSP® Designer. When building complex WebApps and/or
working with large data sets, careful attention should be paid to
optimizing the table structures, indices and SQL views.</span>**

There are many ways to build a DSP® WebApp; however, the optimal method
is by applying Rapid Application Deployment (RAD) for new applications.
This method defines the steps necessary to create a new application,
which are performed with concise and accurate probability.

The following steps apply the RAD philosophy to build DSP® WebApps
quickly:

1.  **Create a Data Source –** Each WebApp in DSP® is based on a
    database. Refer to [Create Tables in SQL](Create_Tables_in_SQL.htm)
    and [Create Views in SQL](Create_Views_in_SQL.htm) for more
    information.
2.  **Create the WebApp** –Refer to [Create a WebApp in
    DSP®](Create_a_WebApp_in_DSP.htm) for more information.
3.  **Register Menus** – *Horizontal* or *Vertical* Menus determine
    where links are available on the current page. Menus can link to
    pages or menus in other WebApps within the site. Refer to [Configure
    the Navigation Pane, Submenus and Links to
    Pages](Configure_the_Navigation_Pane_Submenus_and_Links_to_Pages.htm)
    for more information.
4.  **Register Pages and Assign Page Properties** – Performed through
    page properties, page registration is the foundation of a WebApp and
    contains most of the primary information that controls the web
    environment including security and database connection to tables.
    All pages in the WebApp must be registered to access views. Page
    properties are then assigned to determine page functionality. Refer
    to
    [*<span style="color: #0000ff;">Design</span><span style="color: #0000ff;">Pages</span>*](Page%20Design%20Guidelines.htm)
    for more information.
5.  **Modify Menus** – Update menus to include new pages.
6.  **Assign Column Properties** – Column properties are used to control
    the behavior of fields and how data displays on a page using control
    items, such as list boxes, buttons, labels, page links and images.
    Column properties can be applied to the *Horizontal* View and/or
    *Vertical* View.  Refer to [Assign Column
    Properties](Assign_Column_Properties.htm) for more information.
7.  **Create and Assign Validation Rules** – Validation rules are
    defined through database views and applied to a page or a field.
    Errors or warnings display messages based on the criteria specified
    in the rule. Refer to [Validation Rules](ValidationRules.htm) for
    more information.
8.  **Create and Assign Business Rules** – Corporate business rules can
    be incorporated into a page or a specific field triggering an action
    or event based on a business process. Refer to [Business
    Rules](Business_Rules.htm) for more information.
9.  **Create and Assign Control Views** – Control views provide a way to
    define column control based on what is known about the data, page,
    and/or user. Refer to [Control Views](Control_Views.htm) for more
    information.

Following these steps when designing a new WebApp provides the necessary
details about core functionality as a foundation to deliver a WebApp in
the shortest time possible.
