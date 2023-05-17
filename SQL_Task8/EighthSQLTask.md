# Patika.dev 8.SQL Ödevi 

1.test veritabanınızda employee isimli sütun bilgileri id(INTEGER), name VARCHAR(50), birthday DATE, email VARCHAR(100) olan bir tablo oluşturalım.

`create database test`

`create table employee(employee_id integer primary key not null,name varchar(50) not null,birthday date,email varchar(100) not null)`

2.Oluşturduğumuz employee tablosuna 'Mockaroo' servisini kullanarak 50 adet veri ekleyelim.

`insert into employee(employee_id,name,birthday,email) VALUES (.....)`
`insert into employee(employee_id,name,birthday,email) VALUES (.....)`
`insert into employee(employee_id,name,birthday,email) VALUES (.....)`

3.Sütunların her birine göre diğer sütunları güncelleyecek 5 adet UPDATE işlemi yapalım.

`update employee set name = 'Berkay Öztürk' where employee_id = 1 returning *`
`update employee set email = 'berkay@ozturk.com' where employee_id = 1 returning *`
`update employee set birthday = '2001-12-31' where employee_id = 1 returning *`
`update employee set employee_id = 22 where employee_id = 1 returning *`

4.Sütunların her birine göre ilgili satırı silecek 5 adet DELETE işlemi yapalım.

`Delete from employee where email = 'berkay@oztruk.com`
`Delete from employee where name = 'Berkay Öztürk`
`Delete from employee where birthday = '1980-03-24`
`Delete from employee where employee_id = 10`