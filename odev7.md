# Patika SQL Odev-7

#### 1.*film* tablosunda bulunan filmleri *rating* değerlerine göre gruplayınız.

````roomsql
SELECT rating FROM film
GROUP BY rating
````

#### 2.*film* tablosunda bulunan filmleri *replacement_cost* sütununa göre grupladığımızda film sayısı 50 den fazla olan *replacement_cost* değerini ve karşılık gelen film sayısını sıralayınız.

````roomsql
SELECT replacement_cost FROM film
GROUP BY replacement_cost
HAVING COUNT(replacement_cost)>50
````

#### 3.*customer* tablosunda bulunan *store_id* değerlerine karşılık gelen müşteri sayılarını nelerdir? 

````roomsql
SELECT customer_id, store_id FROM customer
GROUP BY customer_id, store_id
````

#### 4.*city* tablosunda bulunan şehir verilerini *country_id* sütununa göre gruplandırdıktan sonra en fazla şehir sayısı barındıran *country_id* bilgisini ve şehir sayısını paylaşınız.

````roomsql
SELECT country_id FROM city 
GROUP BY country_id
ORDER BY country_id DESC
LIMIT 1;
````