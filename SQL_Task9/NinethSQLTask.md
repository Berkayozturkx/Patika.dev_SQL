# Patika.dev 9.SQL Ödevi 

1.city tablosu ile country tablosunda bulunan şehir (city) ve ülke (country) isimlerini birlikte görebileceğimiz INNER JOIN sorgusunu yazınız.

`select city.city, country.country from city inner join country on city.country_id = country.country_id`

ikinci yol

`select city.city, country.country from city,country where city.country_id = country.country_id`

2.customer tablosu ile payment tablosunda bulunan payment_id ile customer tablosundaki first_name ve last_name isimlerini birlikte görebileceğimiz INNER JOIN sorgusunu yazınız.

`select payment.payment_id,customer.first_name,customer.last_name from customer inner join payment on payment.customer_id = customer.customer_id`

ikinci yol

`select customer.first_name,customer.last_name,payment.payment_id from customer,payment where customer.customer_id = payment.customer_id`

3.customer tablosu ile rental tablosunda bulunan rental_id ile customer tablosundaki first_name ve last_name isimlerini birlikte görebileceğimiz INNER JOIN sorgusunu yazınız.

`select customer.first_name,customer.last_name,rental.rental_id from customer inner join rental on customer.customer_id = rental.customer_id`

ikinci yol

`select customer.first_name,customer.last_name,rental.rental_id from customer,rental where customer.customer_id = rental.customer_id`