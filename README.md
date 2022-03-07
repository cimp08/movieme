# Movieme, an IMBD clone

![](/public/img/mockup.png)

## About the project

This is an imdb-clone where you can register a user, login with your username and use the website as you like. As a user you can add movies to your own watchlist to keep track of your favourite movies. You can also leave reviews on movies so others can see what you thought. As a non-user you can still search for movies and browse all the movies and comments. The admins are able to approve comments, delete comments, add/ edit/ delete movies in the database, delete and edit users. As an admin you can also make regular users admins.

Live version: http://moviemesite.herokuapp.com/

## Built with

-   HTML
-   CSS/ Bootstrap
-   Docker
-   PHP/ Laravel
-   MySQL
-   Heroku

## Get started

1. Clone the repository in your project folder. Docker-compose.yml and Dockerfile is included.
2. Navigate to the root directory of the project and: RUN docker-compose up in your preferred CLI
3. Fix db in .env file using this:

---

DB_CONNECTION=mysql  
DB_HOST=db  
DB_PORT=3306  
DB_DATABASE=movieme  
DB_USERNAME=root  
DB_PASSWORD=example

---

4. Attach a shell and then install composer with "composer install" in the root of the project (cd movieme)
5. Open http://127.0.0.1:8080/ in the browser to view the db, log in using the credentials stated in the third step and when inside create a new database called movieme.
6. Run "php artisan migrate:fresh --seed"
7. Generate your application encryption key using `php artisan key:generate`.
8. Run "php artisan serve --host 0.0.0.0 --port 8000"
9. Open the URL http://127.0.0.1:8000/ in the browser
10. Done!

---

### Admin User to login

Email: admin@test.se
Password: admin1234

---
