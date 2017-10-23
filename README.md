## About This Fork

This fork allows Tomcat web applications to be written and run as Jigsaw modules!
If you put all your dependencies (including your own classes that have to be packed as a modular jar) into `/WEB-INF/modules`
of the resulting WAR file instead of `/WEB-INF/lib` then the jars will be loaded as Jigsaw modules.
Thus `/WEB-INF/modules` stands for complete analog of `--module-path` for web applications.
Note, that jars from `/WEB-INF/lib` are loaded in Unnamed Jigsaw module (regardless of this fork),
thus it is a complete analog of `-cp` for web applications.
So with this fork you can follow the same migration path as suggested by Jigsaw for `-classpath` applications,
gradually moving jars form `/WEB-INF/lib` to `/WEB-INF/modules` modularising your web application this way.

You may try my modular web application example with the fork to see that it actually works:
https://github.com/pjBooms/modular-war-example

## Welcome to Apache Tomcat!

### What Is It?

The Apache Tomcat® software is an open source implementation of the Java
Servlet, JavaServer Pages, Java Expression Language and Java WebSocket
technologies. The Java Servlet, JavaServer Pages, Java Expression Language and
Java WebSocket specifications are developed under the
[Java Community Process](http://jcp.org/en/introduction/overview).

The Apache Tomcat software is developed in an open and participatory
environment and released under the
[Apache License version 2](http://www.apache.org/licenses/). The Apache Tomcat
project is intended to be a collaboration of the best-of-breed developers from
around the world. We invite you to participate in this open development
project. To learn more about getting involved,
[click here](http://tomcat.apache.org/getinvolved.html) or keep reading.

Apache Tomcat software powers numerous large-scale, mission-critical web
applications across a diverse range of industries and organizations. Some of
these users and their stories are listed on the
[PoweredBy wiki page](http://wiki.apache.org/tomcat/PoweredBy).

Apache Tomcat, Tomcat, Apache, the Apache feather, and the Apache Tomcat
project logo are trademarks of the Apache Software Foundation.

### The Latest Version

The current latest version in this branch (trunk) can be found on the [Tomcat 9.0](https://tomcat.apache.org/download-90.cgi) page.

### Documentation

The documentation available as of the date of this release is
included in the docs webapp which ships with tomcat. You can access that webapp
by starting tomcat and visiting http://localhost:8080/docs/ in your browser.
The most up-to-date documentation can be found at
http://tomcat.apache.org/tomcat-9.0-doc/.

### Installation

Please see [RUNNING.txt](RUNNING.txt) for more info.

### Licensing

Please see [LICENSE](LICENSE) for more info.

### Support and Mailing List Information

* Free community support is available through the
[tomcat-users](http://tomcat.apache.org/lists.html#tomcat-users) email list and
a dedicated [IRC channel](http://tomcat.apache.org/irc.html) (#tomcat on
Freenode).

* If you want freely available support for running Apache Tomcat, please see the
resources page [here](http://tomcat.apache.org/findhelp.html).

* If you want to be informed about new code releases, bug fixes,
security fixes, general news and information about Apache Tomcat, please
subscribe to the
[tomcat-announce](http://tomcat.apache.org/lists.html#tomcat-announce) email
list.

* If you have a concrete bug report for Apache Tomcat, please see the
instructions for reporting a bug
[here](http://tomcat.apache.org/bugreport.html).

### Contributing

Please see [CONTRIBUTING](CONTRIBUTING.md) for more info.
