# MySQL on Raspberry Pi / ARM

This is a port of the official MySQL image https://hub.docker.com/_/mysql/ for Raspberry Pi / ARM.

### Supported tags and respective `Dockerfile` links
-	[`5.5`, `latest` (*Dockerfile*)](https://github.com/TobiasH87Docker/rpi-mysql/blob/master/stretch.armhf.5_5.Dockerfile)

### What is MySQL?
MySQL is the world's most popular open source database. With its proven performance, reliability and ease-of-use, MySQL has become the leading database choice for web-based applications, covering the entire range from personal projects and websites, via e-commerce and information services, all the way to high profile web properties including Facebook, Twitter, YouTube, Yahoo! and many more.
For more information and related downloads for MySQL Server and other MySQL products, please visit [MySQL.com](https://www.mysql.com/) or [wikipedia.org/wiki/MySQL](https://en.wikipedia.org/wiki/MySQL)

![logo](https://raw.githubusercontent.com/docker-library/docs/master/mysql/logo.png)

### How to use this image
* ``` $ docker pull tobi312/rpi-mysql ```
* Optional: ``` $ mkdir -p /home/pi/.local/share/mysql ```
* ``` $ docker run --name mysql -d -p 3306:3306 -v /home/pi/.local/share/mysql:/var/lib/mysql -e MYSQL_ROOT_PASSWORD=my-secret-pw tobi312/rpi-mysql ``` 

### Environment Variables
* `TZ` (Default: Europe/Berlin)
* `MYSQL_ROOT_PASSWORD`
* more see: https://hub.docker.com/_/mysql/

### This Image on
* [DockerHub](https://hub.docker.com/r/tobi312/rpi-mysql/)
* [GitHub](https://github.com/Tob1asDocker/rpi-mysql)
