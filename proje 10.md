SQL > Ödev 10

www.patika.dev

1-) city tablosu ile country tablosunda bulunan şehir (city) ve ülke (country) isimlerini birlikte görebileceğimiz LEFT JOIN sorgusunu yazınız.

SELECT city.city, country.country FROM CITY
LEFT JOIN COUNTRY ON country.country_id = city.country_id;

2-) customer tablosu ile payment tablosunda bulunan payment_id ile customer tablosundaki first_name ve last_name isimlerini birlikte görebileceğimiz RIGHT JOIN sorgusunu yazınız.

SELECT customer.first_name, customer.last_name, payment.payment_id FROM payment
RIGHT JOIN customer ON customer.customer_id = payment.customer_id;

3-) customer tablosu ile rental tablosunda bulunan rental_id ile customer tablosundaki first_name ve last_name isimlerini birlikte görebileceğimiz FULL JOIN sorgusunu yazınız.

SELECT customer.first_name, customer.last_name, rental.rental_id FROM rental
FULL JOIN customer ON customer.customer_id = rental.customer_id;
