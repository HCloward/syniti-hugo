+++
title = 'Target Sources – DataServices Connection'
solution = 'Platform'
+++

# Target Sources – DataServices Connection

<div class="use">

Use this page to [configure sources for SAP Data
Services](../Use_Cases/Register_and_Use_Sources#Configure_Source_for_SAP_Data_Services).

</div>

To access this page:

1.  Click <span style="font-weight: bold;">Collect \> Targets</span> in
    the <span style="font-style: italic;">Navigation</span> pane.
2.  Click the <span style="font-weight: bold;">Sources</span> icon for a
    Target.
3.  Click <span style="font-weight: bold;">Vertical View</span> for a
    Source.
4.  Click the <span style="font-weight: bold;">Advanced Settings</span>
    tab.
5.  Click <span style="font-weight: bold;">Connection Settings</span>.

Field available depends on the Data Services Connection Type selected on
the <span style="font-style: italic;">Vertical</span> View  of the
<span style="font-style: italic;">Target Sources</span> page:

  - [ASE15](#ASE15)
  - [DB2 UDBv9](#DB2_UDBv9)
  - [DB2 UDBv8](#DB2_UDBv8)
  - [Informix v10](#Informix_v10)
  - [Informix v11](#Informix_v11)
  - [MySQL v5.0](#MySQL_v5_0)
  - [MySQL v5.1](#MySQL_v5_1)
  - [ODBC](#ODBC)
  - [Oracle10g](#Oracle10g)
  - [Oracle11g](#Oracle11g)
  - [Oracle9i](#Oracle9i)
  - [SAP
Application](#SAP_Application)
  - [SQL2000](#SQL2000)
  - [SQL2005](#SQL2005)
  - [SQL2008](#SQL2008)
  - [SQL2012](#SQL2012)

## <span id="ASE15"></span>ASE15

|                 |                                                                                                                             |
| --------------- | --------------------------------------------------------------------------------------------------------------------------- |
| Field           | Description                                                                                                                 |
| Server          | Displays server and instance name of the database to which Data Services will connect when building or executing a package. |
| User            | Displays user ID to connect to the database.                                                                                |
| Password        | Displays password for user ID to connect to the database.                                                                   |
| Database        | Displays the database name where the source or target tables are stored.                                                    |
| Test Connection | Click to test the connectivity to the database.                                                                             |

## <span id="DB2_UDBv9"></span>DB2 UDBv9

|                 |                                                                 |
| --------------- | --------------------------------------------------------------- |
| Field           | Description                                                     |
| User            | Displays user ID to connect to the database.                    |
| Password        | Displays password for user ID to connect to the database.       |
| ODBC\_DSN       | Displays ODBC data source name used to connect to the database. |
| Test Connection | Click to test the connectivity to the database.                 |

## <span id="DB2_UDBv8"></span>DB2 UDBv8

|                 |                                                                 |
| --------------- | --------------------------------------------------------------- |
| Field           | Description                                                     |
| User            | Displays user ID to connect to the database.                    |
| Password        | Displays password for user ID to connect to the database.       |
| ODBC\_DSN       | Displays ODBC data source name used to connect to the database. |
| Test Connection | Click to test the connectivity to the database.                 |

## <span id="Informix_v10"></span>Informix v10

|                                                   |                                                                 |
| ------------------------------------------------- | --------------------------------------------------------------- |
| Field                                             | Description                                                     |
| User                                              | Displays user ID to connect to the database.                    |
| Password                                          | Displays password for user ID to connect to the database.       |
| <span style="font-weight: bold;">ODBC\_DSN</span> | Displays ODBC data source name used to connect to the database. |
| Test Connection                                   | Click to test the connectivity to the database.                 |

## <span id="Informix_v11"></span>Informix v11

|                 |                                                                 |
| --------------- | --------------------------------------------------------------- |
| Field           | Description                                                     |
| User            | Displays user ID to connect to the database.                    |
| Password        | Displays password for user ID to connect to the database.       |
| ODBC\_DNS       | Displays ODBC data source name used to connect to the database. |
| Test Connection | Click to test the connectivity to the database.                 |

## <span id="MySQL_v5_0"></span>MySQL v5.0

|          |                                                                 |
| -------- | --------------------------------------------------------------- |
| Field    | Description                                                     |
| User     | Displays user ID to connect to the database.                    |
| Password | Displays password for user ID to connect to the database.       |
| odbcDSN  | Displays ODBC data source name used to connect to the database. |

## <span id="MySQL_v5_1"></span>MySQL v5.1

|                 |                                                                 |
| --------------- | --------------------------------------------------------------- |
| Field           | Description                                                     |
| User            | Displays user ID to connect to the database.                    |
| Password        | Displays password for user ID to connect to the database.       |
| ODBC\_DSN       | Displays ODBC data source name used to connect to the database. |
| Test Connection | Click to test the connectivity to the database.                 |

## <span id="ODBC"></span>ODBC

|                 |                                                                 |
| --------------- | --------------------------------------------------------------- |
| Field           | Description                                                     |
| User            | Displays user ID to connect to the database.                    |
| Password        | Displays password for user ID to connect to the database.       |
| ODBC\_DSN       | Displays ODBC data source name used to connect to the database. |
| Test Connection | Click to test the connectivity to the database.                 |

## <span id="Oracle10g"></span>Oracle10g

|                 |                                                                                                                                                                                                                                                                                                                                  |
| --------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Field           | Description                                                                                                                                                                                                                                                                                                                      |
| User            | Displays user ID to connect to the database.                                                                                                                                                                                                                                                                                     |
| Password        | Displays password for user ID to connect to the database.                                                                                                                                                                                                                                                                        |
| Host String     | Displays TNS name or string used to connect to the database using the following format: **\<Oracle\_system\>/\<Oracle\_SID\>**, where **Oracle\_system** is the IP or network name of the system where Oracle is running, and **Oracle\_SID** is the Oracle System identifier that identifies the database on the Oracle system. |
| Test Connection | Click to test the connectivity to the database.                                                                                                                                                                                                                                                                                  |

## <span id="Oracle11g"></span>Oracle11g

|                 |                                                                                                                                                                                                                                                                                                                                                                                                                          |
| --------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Field           | Description                                                                                                                                                                                                                                                                                                                                                                                                              |
| User            | Displays user ID to connect to the database.                                                                                                                                                                                                                                                                                                                                                                             |
| Password        | Displays password for user ID to connect to the database.                                                                                                                                                                                                                                                                                                                                                                |
| Host String     | Displays TNS name or string used to connect to the database using the following format: **\<Oracle\_system\>/\<Oracle\_SID\>**, where <span style="font-weight: bold;">\<</span>**Oracle\_system\>** is the IP or network name of the system where Oracle is running, and <span style="font-weight: bold;">\<</span>**Oracle\_SID\>** is the Oracle System identifier that identifies the database on the Oracle system. |
| Test Connection | Click to test the connectivity to the database.                                                                                                                                                                                                                                                                                                                                                                          |

## <span id="Oracle9i"></span>Oracle9i

|                 |                                                                                                                                                                                                                                                                                                                                  |
| --------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Field           | Description                                                                                                                                                                                                                                                                                                                      |
| User            | Displays user ID to connect to the database.                                                                                                                                                                                                                                                                                     |
| Password        | Displays password for user ID to connect to the database.                                                                                                                                                                                                                                                                        |
| Host String     | Displays TNS name or string used to connect to the database using the following format: **\<Oracle\_system\>/\<Oracle\_SID\>**, where **Oracle\_system** is the IP or network name of the system where Oracle is running, and **Oracle\_SID** is the Oracle System identifier that identifies the database on the Oracle system. |
| Test Connection | Click to test the connectivity to the database.                                                                                                                                                                                                                                                                                  |

## <span id="SAP_Application"></span>SAP Application

|                 |                                                                                                                                                                                                                                                                                                                                  |
| --------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Field           | Description                                                                                                                                                                                                                                                                                                                      |
| Server          | Displays server and instance name of the database to which Data Services will connect when building or executing a package.                                                                                                                                                                                                      |
| User            | Displays user ID to connect to the database.                                                                                                                                                                                                                                                                                     |
| Password        | Displays password for user ID to connect to the database.                                                                                                                                                                                                                                                                        |
| Initial Catalog | Displays the database name used by Data Services to connect to a SQL server.                                                                                                                                                                                                                                                     |
| Host String     | Displays TNS name or string used to connect to the database using the following format: **\<Oracle\_system\>/\<Oracle\_SID\>**, where **Oracle\_system** is the IP or network name of the system where Oracle is running, and **Oracle\_SID** is the Oracle System identifier that identifies the database on the Oracle system. |
| Database        | Displays the database name where the source or target tables are stored.                                                                                                                                                                                                                                                         |
| ODBC\_DSN       | Displays ODBC data source name used to connect to the database.                                                                                                                                                                                                                                                                  |
| Test Connection | Click to test the connectivity to the database.                                                                                                                                                                                                                                                                                  |

## <span id="SQL2000"></span>SQL2000

|                 |                                                                                                                             |
| --------------- | --------------------------------------------------------------------------------------------------------------------------- |
| Field           | Description                                                                                                                 |
| Server          | Displays server and instance name of the database to which Data Services will connect when building or executing a package. |
| User            | Displays user ID to connect to the database.                                                                                |
| Password        | Displays password for user ID to connect to the database.                                                                   |
| Initial Catalog | Displays the database name used by Data Services to connect to a SQL server.                                                |
| Test Connection | Click to test the connectivity to the database.                                                                             |

## <span id="SQL2005"></span>SQL2005

|                 |                                                                                                                             |
| --------------- | --------------------------------------------------------------------------------------------------------------------------- |
| Field           | Description                                                                                                                 |
| Server          | Displays server and instance name of the database to which Data Services will connect when building or executing a package. |
| User            | Displays user ID to connect to the database.                                                                                |
| Password        | Displays password for user ID to connect to the database.                                                                   |
| Initial Catalog | Displays the database name used by Data Services to connect to a SQL server.                                                |
| Test Connection | Click to test the connectivity to the database.                                                                             |

## <span id="SQL2008"></span>SQL2008

|                 |                                                                                                                             |
| --------------- | --------------------------------------------------------------------------------------------------------------------------- |
| Field           | Description                                                                                                                 |
| Server          | Displays server and instance name of the database to which Data Services will connect when building or executing a package. |
| User            | Displays user ID to connect to the database.                                                                                |
| Password        | Displays password for user ID to connect to the database.                                                                   |
| Initial Catalog | Displays the database name used by Data Services to connect to a SQL server.                                                |
| Test Connection | Click to test the connectivity to the database.                                                                             |

## <span id="SQL2012"></span>SQL2012

|                 |                                                                                                                             |
| --------------- | --------------------------------------------------------------------------------------------------------------------------- |
| Field           | Description                                                                                                                 |
| Server          | Displays server and instance name of the database to which Data Services will connect when building or executing a package. |
| User            | Displays user ID to connect to the database.                                                                                |
| Password        | Displays password for user ID to connect to the database.                                                                   |
| Initial Catalog | Displays the database name used by Data Services to connect to a SQL server.                                                |
| Test Connection | Click to test the connectivity to the database.                                                                             |
