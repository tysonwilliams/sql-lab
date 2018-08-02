### Write Basic Queries

- Visit [SQL Try Editor at W3Schools.com](https://www.w3schools.com/Sql/tryit.asp?filename=trysql_select_top) and write the following queries:
  - find all customers with a particular first name.
  ```
  select *
  from Customers
  where ContactName = "Maria Anders";
  ```
  - find all customers that live in London.
  ```
  select *
  from Customers
  where City = "London";
  ```
  - find the phone number for a particular supplier (provide id, or supplier name).
  ```
  select Phone
  from Suppliers
  where SupplierID = 3;
  ```
  - find all customers in a particular postal code.
  ```
  select *
  from Customers
  where PostalCode = 14776;
  ```
  - find all suppliers who have names with more than 20 characters.
  ```
  select *
  from Suppliers
  where length(SupplierName) > 20;
  ```
  - list customers descending by the number of orders.
  ```
  select count(orderID) as numberOfOrders, CustomerName 
    from Orders
    join Customers ON Orders.CustomerID = Customers.CustomerID
  group by Customers.CustomerID
  order by numberOfOrders desc;
  ```
  - list orders descending by the order date.
  ```
  select *
  from Orders
  order by OrderDate desc;
  ```
  - list orders grouped by customer showing the number of orders per customer.
  ```
  
  ```
  - list orders grouped by customer's city showing number of orders per city.
  ```
  
  ```
  - add a customer using your information.
  ```
  
  ```
  - add 2 products.
  ```
  
  ```
  - add 2 orders with you as the customer.
  ```
  
  ```
  - delete all customers that have no orders.
  ```
  
  ```