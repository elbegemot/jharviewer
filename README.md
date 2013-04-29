# JHarviewer #

JHarviewer is [Harviewer](https://github.com/janodvarko/harviewer) packaged as java web app.

Goal is to run harviewer using only Java without PHP required.


## Quick Start ##

Create war

`mvn clean package`

Start server

`java -jar target/jharviewer-standalone.war`

Open url

`http://localhost:8080/jharviewer/`



Notes:
* Embeded Tomcat starts on default 8080 port and with /jharviewer context.
* Content of war will exrtacted to folder .extract in current directory
* To start server on another port use `java -jar target/jharviewer-standalone.war -httpPort=7080`
* Other command line params for Tomcat http://tomcat.apache.org/maven-plugin-2.0/executable-war-jar.html
