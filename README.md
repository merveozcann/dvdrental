# dvdrental
postgresql ödev 1
-- SORU 1

SELECT city,country FROM city
LEFT JOIN country ON city.country_id = country.country_id;

-- SORU 2

SELECT customer.first_name, customer.last_name,payment.payment_id FROM customer
RIGHT JOIN payment ON payment.customer_id = customer.customer_id;

-- SORU 3 

SELECT customer.first_name,customer.last_name, rental.rental_id FROM customer
FULL JOIN rental ON rental.customer_id = customer.customer_id;
