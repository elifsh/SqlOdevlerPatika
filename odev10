# Patika SQL Odev-10

#### 1. *city* tablosu ile *country* tablosunda bulunan şehir (city) ve ülke (country) isimlerini birlikte görebileceğimiz LEFT JOIN sorgusunu yazınız.

````roomsql
SELECT city.city, country.country
FROM city
LEFT JOIN country ON city.country_id = country.country_id;

````

#### 2. *customer* tablosu ile *payment* tablosunda bulunan *payment_id* ile *customer* tablosundaki *first_name* ve *last_name* isimlerini birlikte görebileceğimiz RIGHT JOIN sorgusunu yazınız.

````roomsql
SELECT payment.payment_id, customer.first_name, customer.last_name
FROM payment
RIGHT JOIN customer ON payment.customer_id = customer.customer_id;

````

#### 3. *customer* tablosu ile *rental* tablosunda bulunan *rental_id* ile *customer* tablosundaki *first_name* ve *last_name* isimlerini birlikte görebileceğimiz FULL JOIN sorgusunu yazınız.

````roomsql
SELECT rental.rental_id, customer.first_name, customer.last_name
FROM customer
LEFT JOIN rental ON customer.customer_id = rental.customer_id

UNION

SELECT rental.rental_id, customer.first_name, customer.last_name
FROM rental
LEFT JOIN customer ON rental.customer_id = customer.customer_id
WHERE customer.customer_id IS NULL;

````
