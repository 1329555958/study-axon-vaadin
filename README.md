Sample Axon projects
=====

Rational
-----

This repository aims to gather together a lot of *up-to-date* details spread out on the Internet about:

- frameworks: from [Axon](http://www.axonframework.org/) to Maven Polyglot through [Xtend](https://eclipse.org/xtend/) and other ones;
- miscellaneous know-how: xml free configurations, runnable war, ...

A policy of *Divide and rule* will be used: each main technology or configuration will be presented through a new project.

Each project will provide working code out of the box. No need to know anything other than how to launch Maven should be necessary to run it, i.e.:

- either with Maven and jetty:run,
- or with Java and a standalone jar or war file.

Tools
------

* JDK 1.7 or 1.8

* [Maven](https://maven.apache.org/) (3.2.1 or 3.3.1)

* [Eclipse](https://eclipse.org/) Luna (SR1 or SR2)

* [Jetty](http://eclipse.org/jetty/) 9.2.10

* m2e 1.5.1 (The Maven Integration for Eclipse (m2eclipse)

* Egit 3.7.0

* WikiText 2.3.2

* ...

How to install them is out of the scope of this document.

Key Features
-----

* All the compile/build work is done through Eclipse (m2e). Should you prefer the maven command line, fine.

* Maven Multi-Module with a parent pom module as one of them.

* Persistence with JPA.

* Skip Vaadin Widgetset compilation.

* No package installed in the local m2 repository by any of those projects.

* No specific remote m2 repository is required. Maven Central should be enough.

Steps
------

#### [Legacy project](legacy) ####

This sample application is based upon the [study-axon-vaadin](https://code.google.com/p/study-axon-vaadin/) case study.

#### [Vaadin 7 project](vaadin7) ####

To upgrade to Vaadin 7 requires many changes by itself. It deserves its own project.

#### [Xtend project](xtend) ####

It uses Xtend in place of Java. I should have named it the Low Code Diet!

#### [LowXmlDiet project](lowxmldiet) ####

This kind of diet is possible with the help of Maven Polyglot, Spring Java Configuration, ...

#### [Standalone project](standalone) ####

With the help of *spring-boot-maven-plugin*, create a runable war is a piece of cake.

#### Frendly project ####

Various trics to get a better experience: external configuration, splash screen, shrunken war file, ...

*Work in progress*

Checkout
------

Under Eclipse:

        File > Import... > Git > Projects from Git > Clone URI
using the URL:

        https://github.com/atao60/study-axon-vaadin
        
and the wizard "Import existing Eclipse projects", not the "Import as general project" one.       
        
Building
------        
        
See the README.md file of each module.        

References
------

An article using the original code: [Tutorial - Getting started with CQRS and Axon Framework](http://blog.trifork.com/2010/11/12/tutorial-getting-started-with-cqrs-and-axon-framework/)