# Patika SQL Odev-11

#### 1. *actor* ve *customer* tablolarında bulunan *first_name* sütunları için tüm verileri sıralayalım.

````roomsql
SELECT first_name
FROM actor

UNION

SELECT first_name
FROM customer;


-- İki tablonun first_name sütunları için tüm verileri sıralama
SELECT first_name FROM actor
UNION
SELECT first_name FROM customer;

-- İki tablonun first_name sütunları için kesişen verileri sıralama
SELECT first_name FROM actor
INTERSECT
SELECT first_name FROM customer;


````

#### 2. *actor* ve *customer* tablolarında bulunan *first_name* sütunları için kesişen verileri sıralayalım.

````roomsql
SELECT actor.first_name
FROM actor
INNER JOIN customer ON actor.first_name = customer.first_name;

-- İlk tabloda bulunan ancak ikinci tabloda bulunmayan verileri sıralama
SELECT first_name FROM actor
WHERE first_name NOT IN (SELECT first_name FROM customer);

-- İki tablonun first_name sütunları için tüm verileri sıralama (tekrar edenleri de dahil)
SELECT first_name FROM actor
UNION ALL
SELECT first_name FROM customer;


````

#### 3. *actor* ve *customer* tablolarında bulunan *first_name* sütunları için ilk tabloda bulunan ancak ikinci tabloda bulunmayan verileri sıralayalım.

````roomsql
SELECT actor.first_name
FROM actor
LEFT JOIN customer ON actor.first_name = customer.first_name
WHERE customer.first_name IS NULL;

-- İki tablonun first_name sütunları için kesişen verileri sıralama (tekrar edenleri de dahil)
SELECT first_name FROM actor
INTERSECT ALL
SELECT first_name FROM customer;

-- İlk tabloda bulunan ancak ikinci tabloda bulunmayan verileri sıralama (tekrar edenleri de dahil)
SELECT first_name FROM actor
WHERE first_name NOT IN (SELECT first_name FROM customer)
UNION ALL
SELECT first_name FROM actor
INTERSECT ALL
SELECT first_name FROM customer;


````
