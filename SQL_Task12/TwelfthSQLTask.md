# Patika.dev 12.SQL Ödevi 

1.film tablosunda film uzunluğu length sütununda gösterilmektedir. Uzunluğu ortalama film uzunluğundan fazla kaç tane film vardır?

`select count(film.film_id) as film_sayisi from film where film.length > (select avg(film.length) from film)`

2.film tablosunda en yüksek rental_rate değerine sahip kaç tane film vardır?

`select count(film.film_id) as film_sayisi from film where film.rental_rate = (select max(film.rental_rate) from film)`

3.film tablosunda en düşük rental_rate ve en düşün replacement_cost değerlerine sahip filmleri sıralayınız.

`select * from film where film.rental_rate = (select min(film.rental_rate) from film) and film.replacement_cost = (select min(film.replacement_cost) from film)`

4.payment tablosunda en fazla sayıda alışveriş yapan müşterileri(customer) sıralayınız.

`select payment.customer_id,count(payment.payment_id) as odeme_sayisi from payment group by payment.customer_id order by odeme_sayisi desc`
