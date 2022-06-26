Created web server, application server, and database server. rabbit MQ is used as messaging queue and Memcached as our caching server. whenever a user request comes It hits the Nginx web server and routes this traffic to the application servers. credentials have been configured to log in. All log in go to the Web server 1st and then the web server access the database layer application layer and then the application layer routes the request to the database layer and the database layer verifies the entered credential. the rabbit MQ service takes the request and checks it in-memory cache and if it is not present, routes the request to the database. , created a sample database called accounts. few users have been created to demonstrate from where the data has been fetched, whether it is from the database or it is from the cache for the first time. whenever a request is sent to the database, it first checks in the cache 1st and then goes to the database. once the data is accessed This particular data will be inserted into the cache so that cache will remember those requests, and whenever there is a further similar request. This improves the performance of retrieving the data from the database.  configured reverse proxy server for access.
# Technologies 
 Choclatey
 Oracle virtualbox 
 Vagrant
 Git
 Maven
 MySQL 
 Memcache 
 RabbitMQ 
 Tomcat 
 Nginx 


