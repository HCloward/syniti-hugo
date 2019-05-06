# Business Rule Guidelines

  - Business Rules are stored procedures which are generally created
    from a select view.
  - Common naming for stored procedures is
    webTable\_Event\_Description\#Action where:
      - **Table** – Table registered to the page that calls the business
        rule
      - **Event** – Event that calls the business rule
      - **Description** - Procedure description or field being modified
      - **\#** – An optional number to prevent duplication
      - **Action** – Action performed by stored procedure: 'Upd' if
        update; 'Ins' if insert; 'Del' if delete
  - Name stored procedures that include a select query view the same as
    the select view, without the 'Sel'
    suffix.
    |                  |                                                                     |                             |
    | ---------------- | ------------------------------------------------------------------- | --------------------------- |
    |                  | Governance Example                                                  | Migration Example           |
    | Select View      | webRequestMasterRecipeStepsOperations\_BeforeDelete\_OpPhasesDelSel | webTargetSourceReportUpdSel |
    | Stored Procedure | webRequestMasterRecipeStepsOperations\_BeforeDelete\_OpPhasesDel    | webTargetSourceReportUpd    |
    | Select View      | webRequestPurchasingContractItems\_OnValidate\_PSTYP\_3UpdSel       | webTargetSourceRuleInsSel   |
    | Stored Procedure | webRequestPurchasingContractItems\_OnValidate\_PSTYP\_3Upd          | webTargetSourceRuleIns      |

<!-- end list -->

  - It is recommended to base behavior off of boaStatus rather than
    record existence. To validate data, it must exist; however, if the
    application data is invalid, exceptions during execution could
    result. Considering boaStatus during record manipulation can ensure
    business logic will not fail unexpectedly.

  - Determine under which validation conditions the business rule should
    execute. By default, business rules Run on Validate, which means
    they execute if the record is left in a valid state after the
    Validation Rule’s execution. However, there may be conditions where
    a business rule should ALWAYS execute. For example, a counter on how
    many times a button has been clicked is generally unconcerned with
    record validity and checking both Run on Validate and Run on
    Validate Fail checkboxes on the *Page Business Rules* page’s
    *Vertical* View would enable this. Alternatively, you may want to
    run an event even if the validation fails to record information or
    update a parent record.

  - If using the Force Foreground Execution option on the *Page Business
    Rules* page’s *Vertical* View, be aware that unexpected behavior can
    result. The intent of the feature is to ensure that the Business
    rule runs against the Web Server, even if the event is set to run in
    the background. For example, Force Foreground Execution may be
    required for plugin access to the Http Context. However, depending
    on chain event calling, (as used in Public Web App Events)
    unexpected behavior may result. Additionally, the Business rule
    still runs in the background, even if the Force Foreground Execution
    setting is used, so the Business rule executes twice.

  - Business rules should NEVER throw Internal Errors. Validation rules
    exist to ensure that the expected configuration for success exists
    prior to executing. Any runtime failures that may occur (in other
    words, database connection failures) should be Try/Catch formatted
    typed Messages back to the user.

**NOTE:** The view and stored procedure must have already been created
in SQL.
