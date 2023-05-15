# Patika.dev 2.SQL Ödevi 

1.film tablosunda bulunan tüm sütunlardaki verileri replacement cost değeri 12.99 dan büyük eşit ve 16.99 küçük olma koşuluyla sıralayınız ( BETWEEN - AND yapısını kullanınız.)

`select * from film where film.replacement_cost Between 12.99 and 16.98`

2.actor tablosunda bulunan first_name ve last_name sütunlardaki verileri first_name 'Penelope' veya 'Nick' veya 'Ed' değerleri olması koşuluyla sıralayınız. ( IN operatörünü kullanınız.)

`select actor.first_name, actor.last_name from actor where actor.first_name in('Penelope','Nick','Ed') order by actor.first_name asc`

3.film tablosunda bulunan tüm sütunlardaki verileri rental_rate 0.99, 2.99, 4.99 VE replacement_cost 12.99, 15.99, 28.99 olma koşullarıyla sıralayınız. ( IN operatörünü kullanınız.)

`select * from film where film.rental_rate in (0.99,2.99,4.99) and film.replacement_cost in (12.99,15.99,28.99) order by film.rental_rate, film.replacement_cost asc`