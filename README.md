# JHarviewer #

JHarviewer is [Harviewer](https://github.com/janodvarko/harviewer) packaged as java web app.

Goal is to run harviewer using only Java without PHP required.


## Introduction ##
HAR Viewer is a web application (PHP + Javascript) that allows to visualize HTTP tracing logs based on HTTP Archive format (HAR).
These files contain recorded information about HTTP traffic performed by web pages.
Simplest way create a HAR log file is to use HTTP sniffer tools such as Firebug Net panel.
See [HAR spec] (http://www.softwareishard.com/blog/har-12-spec/) to understand structure of a HAR file.

Ways to create HAR file:
* Export from Firebug
* Using [BrowserMob Proxy](https://github.com/webmetrics/browsermob-proxy) a simple utility that makes it easy to capture performance data from browsers, typically written using automation toolkits such as Selenium and Watir.
* Convert JMeter reports to HAR format using [scripts](https://bitbucket.org/watchmouse/har/)
* Using headless browser PhantomJS and  [network monitoring scripts](https://github.com/ariya/phantomjs/wiki/Network-Monitoring)






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





[![githalytics.com alpha](https://cruel-carlota.pagodabox.com/a89a10b8ec8b8bbef65b2ac49868c9c8 "githalytics.com")](http://githalytics.com/elbegemot/jharviewer)

