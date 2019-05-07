+++
title = 'System Logs'
solution = 'Platform'
+++

# System Logs

<div class="use">

Use this page to:

  - [View system logs](../Use_Cases/View%20System%20Logs.htm)
  - [View a User’s Authentications, Property Changes and Access
    Changes](../Use_Cases/View%20a%20Users%20Auths%20Property%20Access%20Changes.htm)

</div>

To access this page:

1.  Click **Admin \> Resources \> System Logs** in the *Navigation*
    pane.
2.  Click the **Log** icon to view the Access Changes, Authentication
    Attempts, or System Configuration Changes log.

OR

1.  Click **Admin \> Security \> Users** in the Navigation pane.
2.  Click **Vertical View f**or a user.
3.  Click the **View History** icon.

This page contains the following logs:

  - [Access Changes](#Access)
  - [Authentication Attempts](#Authentication)
  - [System Configuration
Changes](#System)

### <span id="Access"></span>Access Changes

|                    |                                                                                |
| ------------------ | ------------------------------------------------------------------------------ |
| Field              | Description                                                                    |
| EVENT LOG ID       | Displays the event log ID.                                                     |
| TIMESTAMP          | Display the date and time the access change was made.                          |
| ENTITY             | Displays the type of entity for which access was changed.                      |
| ENTITY KEY         | Displays the key of the entity for which access was changed.                   |
| ENTITY NAME        | Displays the name of the entity for which access was changed.                  |
| TARGET ENTITY      | Displays the target entity in which access for the entity was changed.         |
| TARGET ENTITY KEY  | Displays the key of target entity in which access for the entity was changed.  |
| TARGET ENTITY NAME | Displays the name of target entity in which access for the entity was changed. |
| RESULT             | Displays the result of the access change.                                      |
| USER               | Displays the name of the user who made the access change.                      |
| SEVERITY           | Displays the severity of the log information.                                  |
| IP ADDRESS         | Displays the IP address of the user who made the access change.                |

### <span id="Authentication"></span>Authentication Attempts

|                        |                                                                                     |
| ---------------------- | ----------------------------------------------------------------------------------- |
| Field                  | Description                                                                         |
| EVENT LOG ID           | Displays the event log ID.                                                          |
| TIMESTAMP              | Display the date and time the authentication attempt was made.                      |
| AUTHENTICATION TYPE    | Displays the type of authentication.                                                |
| AUTHENTICATION KEY     | Displays the authentication key.                                                    |
| AUTHENTICATION USER ID | Displays the ID of the user who attempted authentication.                           |
| RESULT                 | Displays the result of the authentication attempt.                                  |
| RESULT MESSAGE         | Displays the resulting message of the authentication attempt if the attempt failed. |
| SEVERITY               | Displays the severity of the log information.                                       |
| IP ADDRESS             | Displays the IP address of the user that made the authentication attempt.           |

## <span id="System"></span>System Configuration Changes

|              |                                                                             |
| ------------ | --------------------------------------------------------------------------- |
| Field        | Description                                                                 |
| EVENT LOG ID | Displays the event log ID.                                                  |
| TIMESTAMP    | Display the date and time the access change was made.                       |
| ENTITY       | Displays the type of entity for which the configuration change was made.    |
| ENTITY KEY   | Displays the key of the entity for which the configuration change was made. |
| ENTITY NAME  | Displays the entity for which the configuration change was made             |
| FIELD        | Displays the field in which the configuration change was made.              |
| NEW VALUE    | Displays new value of the configuration change.                             |
| RESULT       | Displays the result of the configuration change.                            |
| USER         | Displays the name of the user who made the configuration change.            |
| SEVERITY     | Displays the severity of the log information.                               |
| IP ADDRESS   | Displays the IP address of the user who made the configuration change.      |
