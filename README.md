# sql--dev9
1)city tablosu ile country tablosunda bulunan şehir (city) ve ülke (country) isimlerini birlikte görebileceğimiz INNER JOIN sorgusunu yazınız.
2)customer tablosu ile payment tablosunda bulunan payment_id ile customer tablosundaki first_name ve last_name isimlerini birlikte görebileceğimiz INNER JOIN sorgusunu yazınız.
3)customer tablosu ile rental tablosunda bulunan rental_id ile customer tablosundaki first_name ve last_name isimlerini birlikte görebileceğimiz INNER JOIN sorgusunu yazınız.

1)
SELECT country,city FROM city
INNER JOIN country ON city.country_id=country.country_id;

2)
select customer.first_name,customer.last_name,payment.payment_id from customer
inner join payment on payment.customer_id=customer.customer_id;

3)
select rental.rental_id,customer.first_name,customer.last_name from customer
inner join rental on rental.customer_id=customer.customer_id;
