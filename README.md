# digiblink/jessie-nginx-php5-fpm Docker Container

Maintained by [digiBlink](http://digiblink.eu) - [docker hub link](https://hub.docker.com/r/digiblink/jessie-nginx-php-fpm/)

Container with:

* Debian Jessie (default time zone `Europe/Riga`)
* `nginx` 1.10.3
* PHP-FPM 5.6.33
* `git`

Based on following containers:

* [php](https://hub.docker.com/_/php/)
* [celerative/nginx-php-fpm](https://hub.docker.com/r/celerative/nginx-php-fpm/)

## Usage

To get it running just enter:

`docker run -d --name your_container v /sites/yourdomain.com:/DATA -p 80:80 -t digiblink/jessie-nginx-php5-fpm`

After that you can use BusyBox bash, to log into container: 

`docker exec -ti your_container bash`

After logging in issue following commands:

```
su nginx
wp-cli
```
