# Patika.dev 6.SQL Ödevi 

1.film tablosunda bulunan rental_rate sütunundaki değerlerin ortalaması nedir?

`select round(AVG(film.rental_rate),2) as ortalama_rental_rate from film`

2.film tablosunda bulunan filmlerden kaç tanesi 'C' karakteri ile başlar?`

`select count(*) as c_ile_baslayan_film_sayisi from film where film.title like 'C%'`

3.film tablosunda bulunan filmlerden rental_rate değeri 0.99 a eşit olan en uzun (length) film kaç dakikadır?

`select max(film.length) as en_uzun_film from film where film.rental_rate = 0.99`

4.film tablosunda bulunan filmlerin uzunluğu 150 dakikadan büyük olanlarına ait kaç farklı replacement_cost değeri vardır?

`select count(distinct film.replacement_cost) from film where film.length > 150 `