+++
title = 'Dynamic Views for Multiple Control Fields'
solution = 'Platform'
+++

# Dynamic Views for Multiple Control Fields

This section contains an example of an alternative option to using a
Data Control View to manage the way the fields display on a *Vertical*
View. This method is to only be used when there are many control field
options.

The steps below provide an example of creating Dynamic Views on a page
where a selection in a list box entered on the *Horizontal* view
controls the fields displayed on the *Vertical* View.

Dynamic views are used most effectively on vertical views. The best way
to demonstrate their usefulness is through example.

Refer to [Control Views](Control_Views) for general information.

The Orders table contains the following fields:

  - Fields: **ID** for record ID

  - **Submitted** as date of order

  - **Type** being *Online* or *InStore*

  -  **StoreID** as ID for the store where the order was placed

  - **ShipAddress** for address for shipping online orders

The four views would
be:

|                              |                                               |                                         |                                          |
| ---------------------------- | --------------------------------------------- | --------------------------------------- | ---------------------------------------- |
| webOrdersHor horizontal view | webOrders\#Type\#Ver registered vertical view | webOrders\#Online\#Ver substituted view | webOrders\#InStore\#Ver substituted view |
| ID                           | ID                                            | ID                                      | ID                                       |
| Submitted                    | Submitted                                     | Submitted                               | Submitted                                |
| Type                         | Type                                          |                                         |                                          |
|                              | StoreID                                       |                                         | StoreID                                  |
|                              | ShipAddress                                   | ShipAddress                             |                                          |

 

When the user chooses the **Type** of *Online* on the horizontal view
insert, and then they navigate to the vertical view, the DSP® will look
at the view webOrders\#Type\#Ver and replace the ‘Type’ between the two
\# marks with the value from the table. It will locate
webOrders\#*Online*\#Ver and use that to determine the fields to
display, allowing the user to enter the **ShipAddress** for the Order.

This enables one registered page to enable a few different vertical
views tailored to the content that needs to be displayed.
