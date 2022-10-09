# SqlQuery

***Kodlama.io Yazılım Geliştirici Yetiştirme Kampı - JAVA 2022 3.Hafta'nın 5.ödevidir.<br> https://www.youtube.com/watch?v=r_pbdopB4LU&list=PLqG356ExoxZVN7rC0KmMo0lvECK97VRZg&index=6)<br>
videodaki SQL kodları izlenerek açıklamalı halde uygulanmıştır.*** 


**SELECT - ANSI**

SELECT * FROM Customers

SELECT ContractName, CompanyName, City FROM Customers

SELECT ContractName Adi, CompanyName SirketAdi, City Sehir FROM Customers

SELECT * FROM Customers WHERE City = 'London'

**Case insensitive**

select * from Products where categoryId = 1 or categoryId= 3

SELECT * FROM Products WHERE categoryId = 1 AND UnitPrice >= 10

SELECT * FROM Products ORDER BY ProductName

SELECT * FROM Products ORDER BY CategoryId, ProductName

**ascending**

SELECT * FROM Products ORDER BY UnitPrice asc  

**descending**

SELECT * FROM Products ORDER BY UnitPrice desc

SELECT * FROM Products where categoryId = 1 ORDER BY UnitPrice desc

SELECT COUNT(*) from Products

SELECT COUNT(*) from Products where CategoryId = 2 

SELECT COUNT(*) Adet from Products where CategoryId = 2

SELECT * FROM products GROUP BY CategoryId 

SELECT categoryId FROM products GROUP BY CategoryId

SELECT categoryId, COUNT(*) FROM products WHERE UnitPrice > 20 GROUP BY CategoryId HAVING COUNT(*) < 10

SELECT Products.ProductId, Products.ProductName, Products.UnitPrice, Categories.Categoryname FROM Products INNER JOIN Categories ON Products.CategoryId = Categories.CategoryId

**DATA TRANSFORMATION OBJECT**

Select * from Products p inner join [Order Details] od on p.ProductId = od.ProductId

Select * from Products p left join [Order Details] od on p.ProductId = od.ProductId

Select * from Customers c left join Orders o on c.CustomerId = o.CustomerId where o.CustomerId is null

Select * from Customers c right join Orders o on C.CustomerId = o.CustomerId where o.CustomerId is null







- Alias kullanılarak istenilen alanların çekilmesi <br>
`select ContactName Adi, CompanyName SirketAdi,City Sehir  from Customers`


