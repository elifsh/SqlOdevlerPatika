# Patika SQL Odev-9

#### 1. *city* tablosu ile *country* tablosunda bulunan şehir (city) ve ülke (country) isimlerini birlikte görebileceğimiz INNER JOIN sorgusunu yazınız.


````roomsql
SELECT city.Name AS CityName, country.Name AS CountryName
FROM city
INNER JOIN country ON city.CountryCode = country.CountryCode;

````

#### 2. *customer* tablosu ile *payment* tablosunda bulunan *payment_id* ile *customer* tablosundaki *first_name* ve *last_name* isimlerini birlikte görebileceğimiz INNER JOIN sorgusunu yazınız.

````roomsql
SELECT payment.payment_id, customer.first_name, customer.last_name
FROM payment
INNER JOIN customer ON payment.customer_id = customer.customer_id;
````

#### 3. *customer* tablosu ile *rental* tablosunda bulunan *rental_id* ile *customer* tablosundaki *first_name* ve *last_name* isimlerini birlikte görebileceğimiz INNER JOIN sorgusunu yazınız.

````roomsql
SELECT rental.rental_id, customer.first_name, customer.last_name
FROM rental
INNER JOIN customer ON rental.customer_id = customer.customer_id;

````

