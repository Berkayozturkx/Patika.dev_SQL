# Patika.dev 7.SQL Ödevi 

1.film tablosunda bulunan filmleri rating değerlerine göre gruplayınız.

`select film.rating from film group by film.rating`

2.film tablosunda bulunan filmleri replacement_cost sütununa göre grupladığımızda film sayısı 50 den fazla olan replacement_cost değerini ve karşılık gelen film sayısını sıralayınız.

`select film.replacement_cost,count(film.film_id) as film_sayisi from film group by film.replacement_cost having count(film.film_id) > 50`

3.customer tablosunda bulunan store_id değerlerine karşılık gelen müşteri sayılarını nelerdir?

`select customer.store_id,count(customer.customer_id) as musteri_sayisi from customer group by customer.store_id`

4.city tablosunda bulunan şehir verilerini country_id sütununa göre gruplandırdıktan sonra en fazla şehir sayısı barındıran country_id bilgisini ve şehir sayısını paylaşınız.

`select country.country_id as ulke_numarasi, count(city.city_id) as sehir_sayisi from city,country where city.country_id = country.country_id group by country.country_id order by sehir_sayisi desc limit 1`