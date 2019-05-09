+++
title = 'Create Events'
solution = 'Platform'
+++

# Create Events

Events are actions that contain validation rules and/or business rules.
Validation rules run first and validate data before executing any rules.
Business rules run after validation rules complete and perform an
action. They can be incorporated into each page or for a specific field
triggering an action or event. Validation rules always run in the
foreground; however, business rules can be specified to run in the
foreground or in the background, depending on the complexity.

  - **Foreground Events** – Events selected to run in the foreground
    execute immediately when the status icon is clicked and the page
    refreshes.
  - **Background Events** – Business rules that take a longer time to
    run can be forced to run in the background. Background events are
    placed into a job queue for later execution. The status is queued
    when the rule is first submitted. When the event is running, the
    boaStatus becomes Executing (11). It then becomes Execution Failed
    (12) or Complete (4).

Event rules can be created to run:

  - **OnLoad** – Executes prior to the page displaying allowing lazy
    data population.
    
    **NOTE:** This event rule is not available for Service pages.

  - **OnValidate** – Executes when a record is saved or the boaStatus
    icon is clicked.
    
    **NOTE:** This event rule is not available for Report pages.

  - **BeforeDelete** – Executes before a record can officially be
    deleted.
    
    **NOTE:** BeforeDelete events can be run in the Background only.
    
    **NOTE:** This event rule is not available for Service pages.

  - **Columns** – Executes at the record level from clicking a specific
    field. The options display as the names of the columns that can have
    record-level events added.

There are two ways to add events in DSP:

  - Log in to System Administration, navigate to WebApps, locate the
    WebApp and click **Pages**. Locate the page and click **Events**.
  - Navigate to the page in the WebApp where the column property is to
    be applied. Click the **Change Settings** icon on the Site toolbar,
    click **Design**, then click **Events**.

This section contains these topics:

  - [Event Design Process](Event_Design_Process)
  - [OnLoad Events](OnLoad_Events)
  - [OnValidate Events](OnValidate_Events)
  - [Validation Rules](ValidationRules)
  - [Business Rules](Business_Rules)
  - [Set Parameters for a Public WebApp Event](Set_Param_Public)
