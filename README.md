# Database9

select customers.customerName, offices.city as office_city from customers, employees, offices where customers.salesRepEmployeeNumber = employees.employeeNumber and employees.officeCode = offices.officeCode and customers.city = offices.city;

1. Rewrite it as an expression in relational algebra
2. Add row counts to the subexpressions
3. Rewrite to a better expression



a1. Rewritting the query to algebra relation. Select the markdown and put the query between 2 dollarsigns $.

?officecity/office.city(ssalesRepEmployeeNumber=employeeNumber(customers122×(employees23?offices7)))?officecity/office.city(ssalesRepEmployeeNumber=employeeNumber(customers122×(employees23?offices7)))

![image](https://i.imgur.com/iBa9lR0.png)


a2 Adding row account.
\Pi_{customerName,office\_city}(\rho_{office\_city/office.city}(\sigma_{salesRepEmployeeNumber=employeeNumber}(customers^{122}\times (employees^{23}\bowtie offices^{7})^{23} )^{2806} )^{14})

![image](https://i.imgur.com/UABA8li.png)

a3 Rewritting the query to a better expression.
\Pi_{customerName,office_city}(\rho_{office_city/office.city}((\sigma_{salesRepEmployeeNumber=employeeNumber}(customers^{122}\times employees^{23}))^{14}\bowtie offices^{7})^{14})

![image](https://i.imgur.com/xpxT9El.png)

