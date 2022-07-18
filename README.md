# SQL11

Aşağıdaki sorgu senaryolarını dvdrental örnek veri tabanı üzerinden gerçekleştiriniz.

1. actor ve customer tablolarında bulunan first_name sütunları için tüm verileri sıralayalım.

(SELECT actor.first_name FROM actor) UNION (SELECT customer.first_name FROM customer);

2. actor ve customer tablolarında bulunan first_name sütunları için kesişen verileri sıralayalım.

(SELECT actor.first_name FROM actor) INTERSECT (customer.first_name FROM customer);

3. actor ve customer tablolarında bulunan first_name sütunları için ilk tabloda bulunan ancak ikinci tabloda bulunmayan verileri sıralayalım.

(SELECT actor.first_name FROM actor) EXCEPT (customer.first_name FROM customer);

4. İlk 3 sorguyu tekrar eden veriler için de yapalım.

(SELECT actor.first_name FROM actor) UNION ALL (SELECT customer.first_name FROM customer);

(SELECT actor.first_name FROM actor) INTERSECT ALL (SELECT customer.first_name FROM customer);

(SELECT actor.first_name FROM actor) EXCEPT ALL (SELECT customer.first_name FROM customer);
