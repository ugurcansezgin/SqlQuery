# SqlQuery

***Kodlama.io Yazılım Geliştirici Yetiştirme Kampı - JAVA 2022 3.Hafta'nın 5.ödevidir.<br> https://www.youtube.com/watch?v=r_pbdopB4LU&list=PLqG356ExoxZVN7rC0KmMo0lvECK97VRZg&index=6)<br>
videodaki SQL kodları izlenerek açıklamalı halde uygulanmıştır.*** 

- Alias kullanılarak alanların çekilmesi <br>
`SELECT ContactName Adi, CompanyName SirketAdi,City Sehir  FROM Customers`

- Alias olmadan çekilmesi <br>
`SELECT ContactName, CompanyName, City FROM Customers`

- Filtreleme <br>
`SELECT * FROM Customers WHERE City ='London'`

- (case insensitive) küçük-büyük harf ayırmaksızın kodu çalıştırma <br>
`select * from Products where CategoryId = 1 or CategoryId = 3`<br>
`select * from Products where CategoryId = 1 and UnitPrice = 10`

- asc (artan şekilde sıralama) <br>
`Select * from Products order by UnitPrice asc`

- desc (azalan şekilde sıralama) <br>
`Select * from Products order by UnitPrice desc`

- COUNT -> Tabloda kaç adet veri olduğunu bulmak <br>
`Select count(*) from Products`

- Data Transformaiton Object -> İstenilen alanların çekilmesi <br>
- INNER JOIN -> İki tabloda da ortak olan verileri alma işlemi <br>
`Select * from Products p inner join [Order Details] od on p.ProductId = od.ProductId`



