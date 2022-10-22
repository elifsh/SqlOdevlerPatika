# Patika SQL Odev-6

#### 1.*film* tablosunda bulunan *rental_rate* sütunundaki değerlerin ortalaması nedir?

````roomsql
SELECT ROUND(AVG(rental_rate),3) FROM film 
````

#### 2.*film* tablosunda bulunan filmlerden kaç tanesi 'C' karakteri ile başlar?

````roomsql
SELECT COUNT(title) FROM film
WHERE title LIKE 'C%'
````

#### 3.*film* tablosunda bulunan filmlerden *rental_rate* değeri 0.99 a eşit olan en uzun (*length*) film kaç dakikadır?

````roomsql
SELECT MAX(length) FROM film
WHERE rental_rate = 0.99
````

###### ya da şöyle yapılabilir:

````roomsql
SELECT * FROM film
WHERE rental_rate = 0.99
ORDER BY length DESC
LIMIT 1;
````

#### 4.*film* tablosunda bulunan filmlerin uzunluğu 150 dakikadan büyük olanlarına ait kaç farklı *replacement_cost* değeri vardır?

````roomsql
SELECT COUNT(DISTINCT replacement_cost) FROM film
WHERE length >= 150 
````