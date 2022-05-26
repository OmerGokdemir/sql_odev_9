# sql_odev_9
SQL 9. Ödevi

## Aşağıdaki sorgu senaryolarını *dvdrental* örnek veri tabanı üzerinden gerçekleştiriniz.

1. *city* tablosu ile *country* tablosunda bulunan şehir (*city*) ve ülke (*country*) isimlerini birlikte görebileceğimiz INNER JOIN sorgusunu yazınız.

```SQL
      SELECT city, country FROM city
      INNER JOIN country ON city.country_id = country.country_id;
```

2. *customer* tablosu ile *payment* tablosunda bulunan *payment_id* ile *customer* tablosundaki *first_name* ve *last_name* isimlerini birlikte görebileceğimiz INNER JOIN sorgusunu yazınız.

```SQL
      SELECT payment_id, first_name, last_name FROM payment
      INNER JOIN customer ON payment.customer_id = customer.customer_id;
```

3. *customer* tablosu ile *rental* tablosunda bulunan *rental_id* ile *customer* tablosundaki *first_name* ve *last_name* isimlerini birlikte görebileceğimiz INNER JOIN sorgusunu yazınız.

```SQL
      SELECT rental_id, first_name, last_name FROM rental
      INNER JOIN customer ON rental.customer_id = customer.customer_id;
```
