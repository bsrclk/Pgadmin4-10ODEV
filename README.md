# Pgadmin4-10ODEV
10.ÖDEV

--10.ÖDEV

--1.)city tablosu ile country tablosunda bulunan şehir (city) ve ülke (country) isimlerini birlikte görebileceğimiz LEFT JOIN sorgusunu yazınız.

select city_id ,country.country_id,city.country_id,city,country from city
left join country on city.country_id=country.country_id

--2.)customer tablosu ile payment tablosunda bulunan payment_id ile customer tablosundaki first_name ve last_name isimlerini birlikte görebileceğimiz RIGHT JOIN sorgusunu yazınız.

select payment_id,first_name,last_name,payment.customer_id,customer.customer_id from customer
left join payment on payment.customer_id=customer.customer_id

--3.)customer tablosu ile rental tablosunda bulunan rental_id ile customer tablosundaki first_name ve last_name isimlerini birlikte görebileceğimiz FULL JOIN sorgusunu yazınız.

select rental_id,rental.customer_id,customer.customer_id,first_name,last_name from customer
full join  rental on rental.customer_id=customer.customer_id
