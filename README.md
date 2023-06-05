# patika_academy_project_sql6
query scenarios

Perform the following query scenarios on the "dvdrental" sample database.

1. What is the average of the values in the "rental_rate" column in the movie table?

SELECT AVG (rental_rate) FROM film;

2. How many of the movies in the movie table start with the character 'C'?

SELECT COUNT (title) FROM film

WHERE title LIKE 'C%';

3. How many minutes is the longest (length) movie whose "rental_rate" value is equal to 0.99 among the movies in the movie table?

SELECT MAX (length) FROM film

WHERE rental_rate=0.99;

4. How many different "replacement_cost" values are there for the movies longer than 150 minutes in the movie table?

SELECT COUNT (DISTINCT replacement_cost) FROM film

WHERE length>150;
