## LAB 1

Lab Assignment 1

Part 1 (7.5 pts)
For this project, you’ll create a form that lets the user maintain products using a DataGridView control.
The design of the Product Maintenance form

Operation
 When this application starts, all the rows in the Products table of the TechSupport database are
displayed in the DataGridView control.
 The user can use the toolbar and the DataGridView control to add new rows, delete rows, modify the
data in existing rows, and save changes to the database.

Specifications
 This application should handle SQL Server exceptions, ADO.NET exceptions, and data errors that
occur when working with the DataGridView control.

Part 2 (7.5 pts)
The design of the Technician Maintenance form

Operation
 When this application first starts, the data in the first row of the Technicians table is displayed. Then, the
user can display the data for other rows using the navigation buttons in the toolbar.
 To modify an existing row, the user enters the modifications and then clicks the Save Data button in the
toolbar.
 To delete an existing row, the user clicks the Delete button in the toolbar, followed by the Save Data
button.
 To add a new row, the user clicks the Add New button in the toolbar, enters the data for the new row,
and then clicks the Save Data button.

Specifications
 This application should handle SQL Server and ADO.NET exceptions.
 Because the TechID column is an identity column, don’t allow the user to change the value in this
column.
 Limit the number of characters that can be entered into the Name, Email, and Phone text boxes so the
entries don’t exceed the sizes allowed by the Name, Email, and Phone columns.
