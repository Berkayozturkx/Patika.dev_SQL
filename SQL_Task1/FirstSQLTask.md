# Patika.dev 1.SQL Ödevi

1.film tablosunda bulunan title ve description sütunlarındaki verileri sıralayınız.

`select title,description from film`

2.film tablosunda bulunan tüm sütunlardaki verileri film uzunluğu (length) 60 dan büyük VE 75 ten küçük olma koşullarıyla sıralayınız.

`select * from film where film.length > 60 and film.length < 75`

ikinci yol

`select * from film where film.length between 61 and 75`

3.film tablosunda bulunan tüm sütunlardaki verileri rental_rate 0.99 VE replacement_cost 12.99 VEYA 28.99 olma koşullarıyla sıralayınız.

`select * from film where film.rental_rate = 0.99 and (film.replacement_cost = 12.99 or film.replacement_cost = 28.99)`

4.customer tablosunda bulunan first_name sütunundaki değeri 'Mary' olan müşterinin last_name sütunundaki değeri nedir?

`select first_name,last_name from customer where customer.first_name = 'Mary'`

5.film tablosundaki uzunluğu(length) 50 ten büyük OLMAYIP aynı zamanda rental_rate değeri 2.99 veya 4.99 OLMAYAN verileri sıralayınız.

`select * from film where not (film.length = 50) and not (film.rental_rate = 2.99 or film.rental_rate = 4.99)`