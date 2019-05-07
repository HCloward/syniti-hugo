+++
title = 'Plugin API Functionality'
solution = 'Platform'
+++

# Plugin API Functionality

The following API functionality is helpful to know and understand when
coding the plugin:

  - [Connect to the database](#ConnectToTheDatabase)
  - [Read from the database](#ReadFromTheDatabase)
  - [Write to the database](#WriteToTheDatabase)

## <span id="ConnectToTheDatabase"></span>Connect to the Database

The mechanism by which the plugin connects to the database is an
IDataService object. To establish a connection to the database, create a
new instance of the IDataService object and use the Host.GetDataService
method.

### C\# Example

Use the following C\# command to establish a connection between the
plugin and the page’s Data Source.

![](../../../Resources/Images/Plugin%20API%20Functionality_1.png)

![](../../../Resources/Images/Plugin%20API%20Functionality_2.png)

### Visual Basic .Net Example

Use the following Visual Basic .Net command to establish a connection
between the plugin and the page’s Data Source.

![](../../../Resources/Images/Plugin%20API%20Functionality_3.png)

## <span id="ReadFromTheDatabase"></span>Read From the Database

With a connection established, the IDataService object can be used to
read from the database. There are many functions that can be used to
read from the database.

### C\# Example

Use one of the following two most commonly used C\# functions to read
from a database.

![](../../../Resources/Images/Plugin%20API%20Functionality_4.png)

### Visual Basic.Net Example

Use one of the following two most commonly used Visual Basic.Net
functions to read from a database.

![](../../../Resources/Images/Plugin%20API%20Functionality_5.png)

## <span id="WriteToTheDatabase"></span>Write to the Database

With a connection established, the IDataService object can be used to
write to the database. There are many functions that can be used to
write to the database; the most commonly used function is
ExecuteNonQuery.

### C\# Example

Use the ExecuteNonQuery function to write to the database.

![](../../../Resources/Images/Plugin%20API%20Functionality_6.png)

### Visual Basic .Net Example

Use the ExecuteNonQuery function to write to the database.

![](../../../Resources/Images/Plugin%20API%20Functionality_7.png)
