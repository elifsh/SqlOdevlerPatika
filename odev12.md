# Patika SQL Odev-12

#### 1. *film* tablosunda film uzunluğu *length* sütununda gösterilmektedir. Uzunluğu ortalama film uzunluğundan fazla kaç tane film vardır?

````roomsql
-- Ortalama film uzunluğunu bulma
SELECT AVG(length) AS ortalama_uzunluk
FROM film;

-- Ortalama uzunluğundan daha uzun kaç film olduğunu bulma
SELECT COUNT(*) AS film_sayisi
FROM film
WHERE length > (SELECT AVG(length) FROM film);

````

#### 2. *film* tablosunda en yüksek *rental_rate* değerine sahip kaç tane *film* vardır?

````roomsql
SELECT COUNT(*) AS film_sayisi
FROM film
WHERE rental_rate = (SELECT MAX(rental_rate) FROM film);

````

#### 3. *film* tablosunda en düşük *rental_rate* ve en düşün *replacement_cost* değerlerine sahip filmleri sıralayınız.

````roomsql
SELECT *
FROM film
WHERE rental_rate = (SELECT MIN(rental_rate) FROM film)
  AND replacement_cost = (SELECT MIN(replacement_cost) FROM film);

````

#### 4. *payment* tablosunda en fazla sayıda alışveriş yapan müşterileri(customer) sıralayınız.

````roomsql
SELECT customer_id, COUNT(*) AS toplam_alisveris
FROM payment
GROUP BY customer_id
ORDER BY toplam_alisveris DESC;

````
