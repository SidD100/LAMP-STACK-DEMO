### Description

Get a LAMP stack project up and running in 10 mins!

### Requirements
- IDE (eg.: VSCode)
- Docker
- Browser (eg.: Firefox)

To run this code, 
1. Clone the repo.
2. Open command line in the same directory
3. Open Docker, navigate to Containers
4. Run `docker-compose up` in the CLI
5. Open a browser to [view the table](localhost:80) and [view PHPMyAdmin page](localhost:8081)


### NOTE
Once you get the error: <br />

>Fatal error: Uncaught Error: Call to undefined function mysqli_connect() in /var/www/html/index.php:3 Stack trace: #0 {main} thrown in /var/www/html/index.php on line 3  


Go to Docker's '**www**' server's interactive terminal and run `docker-php-ext-install mysqli && docker-php-ext-enable mysqli && apachectl restart` <br />

### Credits
Inspired from Vincent Stevenson's [Build a Full Stack Web App in PHP and MySQL with Docker from scratch!](https://youtu.be/2Bxh5FNGznQ).
