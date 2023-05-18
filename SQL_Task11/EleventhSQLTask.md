# Patika.dev 11.SQL Ödevi 

1.actor ve customer tablolarında bulunan first_name sütunları için tüm verileri sıralayalım.

`(select actor.first_name from actor) union (select customer.first_name from customer)`

2.actor ve customer tablolarında bulunan first_name sütunları için tüm verileri tekrar eden veriler için de sıralayalım.

`(select actor.first_name from actor) union all (select customer.first_name from customer)`

3.actor ve customer tablolarında bulunan first_name sütunları için kesişen verileri sıralayalım.

`(select actor.first_name from actor) INTERSECT (select customer.first_name from customer)`

4.actor ve customer tablolarında bulunan first_name sütunları için kesişen verileri tekrar eden tüm veriler için de sıralayalım.

`(select actor.first_name from actor) INTERSECT ALL (select customer.first_name from customer)`

5.actor ve customer tablolarında bulunan first_name sütunları için ilk tabloda bulunan ancak ikinci tabloda bulunmayan verileri sıralayalım.

`(select actor.first_name from actor) EXCEPT (select customer.first_name from customer)`

6.actor ve customer tablolarında bulunan first_name sütunları için ilk tabloda bulunan ancak ikinci tabloda bulunmayan verileri tekrar eden veriler için de sıralayalım.

`(select actor.first_name from actor) EXCEPT ALL (select customer.first_name from customer)`