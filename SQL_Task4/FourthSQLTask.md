# Patika.dev 4.SQL Ödevi 

1.film tablosunda bulunan replacement_cost sütununda bulunan birbirinden farklı değerleri sıralayınız.

`select distinct film.replacement_cost from film'`

2.film tablosunda bulunan replacement_cost sütununda birbirinden farklı kaç tane veri vardır?

`select count(distinct film.replacement_cost) as farkli_veri_sayisi from film`

3.film tablosunda bulunan film isimlerinde (title) kaç tanesini T karakteri ile başlar ve aynı zamanda rating 'G' ye eşittir?

`select count(film.film_id) as film_sayisi from film where film.title like 'T%'and film.rating = 'G'`

4.country tablosunda bulunan ülke isimlerinden (country) kaç tanesi 5 karakterden oluşmaktadır?

`select count(country.country_id) as ulke_sayisi from country where country.country like '_____'`

5.city tablosundaki şehir isimlerinin kaç tanesi 'R' veya r karakteri ile biter?

`select count(country.country_id) as ulke_sayisi from country where (country.country like '%R' or country.country like '%r')`