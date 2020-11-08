# Simple Java
[![Hits](https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2Fangryziber%2Fsimple-java&count_bg=%2379C83D&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=PAGE+VIEWS&edge_flat=false)](https://hits.seeyoufarm.com)

This is a skeleton project for a Java webapp, done right.

It includes:
- Ant & Ivy for dependency management
- Jersey for handling of http requests in a RESTful way
- Spring for dependency injection in the code
- H2 database (Windows users may need to edit jetty-web.xml)
- Liquibase for DB migration
- Hibernate for working with the DB
- JUnit & Mockito for unit testing

After cloning, run src/Launcher.java to start. Everything is preconfigured.

Small amount of code it contains implements a simple database of good Photo Spots,
which uses google maps to browse and edit them.

Or you can follow how this all have been created by pulling various branches
into your own branch in this order:
- start - empty project
- ivy - add ivy for dependency management
- launcher - adds Jetty launcher to run the app without any external application servers
- map - adds html with Google Map
- web.xml - first step for Java web app
- logging - adds good logging, useful for any web app
- jersey - adds Jersey (JAX-RS implementation) for handling HTTP REST requests
- map-with-spots - adds dummy photo spots to the Google Map
- add-spot - possibility to add new spots to the map
- spring - adds Spring for dependency injection
- db - adds H2 database
- hibernate - adds Hibernate for persisting of objects without hand-coded JDBC code
- tests - adds some unit tests (in real life these should be added on every step)
- db-testing - adds plain JDBC implementation for persistence as well as more tests, see 2nd presentation below

By following these branches in this order you can also get an idea how to build an app step-by-step,
following Just Enough Design principle.

See related talk from GOTOCon and Devclub here - "How to get Java back":
http://www.slideshare.net/antonkeks/simplicity-8971441

And another one about DB testing from Topconf - "3 tales of testing of DB-enabled apps":
http://prezi.com/kq0ghszq6e-j/3-tales-of-testing-db-enabled-apps/
