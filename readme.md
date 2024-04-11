# petclinic-jakartaee

![Jakarta EE Compatible](src/main/webapp/img/logos/Jakarta_10__22_09_2022.jpg)

Petclinic Jakarta EE - a Jakarta EE 10 Version of Spring Petclinic demo application using PrimeFaces JSF.

![Jakarta EE Compatible](src/main/webapp/img/logos/home_logo_jakartaee.png)

To Access the Deployed Application, Click on Below Link:
https://cli-demo-0547af24.payara.app/petclinic-jakartaee/home.jsf

For Blog: https://blog.payara.fish/deploying-to-payara-cloud-from-a-github-action-workflow

## What is this?
* JSF and Jakarta EE 10 Version of [Spring Petclinic](https://github.com/spring-projects/spring-petclinic)
* This is an Update of [Java EE 7 Petclinic](https://jakarta-ee-petclinic.github.io/petclinic-javaee7/)

## Where is it?
* Github: [https://github.com/Jakarta-EE-Petclinic/petclinic-jakartaee](https://github.com/Jakarta-EE-Petclinic/petclinic-jakartaee)
* Demo on OpenShift: [http://jakartaee8petclinic.rhcloud.com/](http://jakartaee8petclinic.rhcloud.com)
* Blog: [https://thomas-woehlke.blogspot.com/2014/02/java-ee-7-petclinic.html](https://thomas-woehlke.blogspot.com/2014/02/java-ee-7-petclinic.html)

## Motivation
* Some experimental Work with JSF, Jakarta EE 10 and Java EE 
* This Demo Application is planned to be the first in a series of “Rosetta Stone” to compare OOP Web Application Frameworks

## Why Petclinic?
* The Domain Classes show all relationships like one-to-many (1:n), many-to-one (n:1) and many-to-many (n:m)
* It is simple enough but yet it shows more than just the CRUD Use Cases (Create, Read, Update, Delete) of most Demos and Training Examples.
* You can think of it as smallest complete Web App with the usual things to solve.

## About Java EE 7 Petclinic
* [github.com/Jakarta-EE-Petclinic/petclinic-javaee7](https://github.com/Jakarta-EE-Petclinic/petclinic-javaee7)
* [Thomas Woehlke: Java EE 7 Petclinic](https://thomas-woehlke.blogspot.com/2014/02/java-ee-7-petclinic.html)
* [Stefan Hildebrandt: Was eine QS-Abetilung immer wollte. Mit automatisierten Tests zum Ziel](https://consulting.hildebrandt.tk/vortraege/integrierteAkzeptanztests/slides/index.html#/)
* [Reza Rahman: Migrating the Spring Pet Clinic to Java EE 7](https://dzone.com/articles/migrating-spring-pet-clinic)

### Spring Petclinic
* Github: [https://github.com/spring-projects/spring-petclinic](https://github.com/spring-projects/spring-petclinic)

## dev, build ...

```
git clone git@github.com:Jakarta-EE-Petclinic/petclinic-jakartaee.git
cd petclinic-jakartaee
./mvnw
```

## ... deploy and run

| maven profile      | Runtime                                                               | Version      | Status         |
|--------------------|-----------------------------------------------------------------------|--------------|----------------|
| ./mvnw -Pliberty   | [OpenLiberty](https://openliberty.io/)                                | 23.0.0.6     | Jakarta EE 10  |
| ./mvnw -Pwildfly   | [Wildfly](https://www.wildfly.org/)                                   | 28.0.1.Final | Jakarta EE 10  |
| ./mvnw -Ppayara    | [Payara](https://www.payara.fish/products/payara-platform-community/) | 6.2023.6     | Jakarta EE 10  | 
| ./mvnw -Pglassfish | [GlassFish](https://glassfish.org/)                                   | 7.0.5        | Jakarta EE 10  |
| ./mvnw -Ptomee     | [Apache TomEE](https://tomee.apache.org/)                             | 9.1.0        | Jakarta EE 9.1 |


## Integration Tests

Arquillian End2End Tests for REST Endpoints and for JSF Frontend Browser Tests with Graphene and Selenium.
* [JSF, Java Server Faces: Primefaces 12.0.0](https://www.primefaces.org/)

| maven profile                  | Runtime                                                                  | Version      | Status                  |
|--------------------------------|--------------------------------------------------------------------------|--------------|-------------------------|
| ./mvnw -Parq-liberty-managed   | [OpenLiberty](https://openliberty.io/docs/latest/overview.html)          | 23.0.0.1     | waiting for OpenLiberty |
| ./mvnw -Parq-wildfly-managed   | [Wildfly](https://docs.wildfly.org/27/)                                  | 27.0.1.Final | work in progress        |
| ./mvnw -Parq-payara-managed    | [Payara](https://docs.payara.fish/community/docs/6.2022.1/Overview.html) | 6.2023.2     | work in progress        | 
| ./mvnw -Parq-glassfish-managed | [GlassFish](https://glassfish.org/documentation)                         | 7.0.2        | work in progress        |



## References

### Jakarta EE Runtimes 
* [Wildfly](https://www.wildfly.org/)
* [Open Liberty](https://openliberty.io/)
* [Eclipse GlassFish](https://glassfish.org/h)
* [Payara Server](https://www.payara.fish/)
* [Apache TomEE](https://tomee.apache.org/)
* [JSF Java Server Faces: Primefaces](https://www.primefaces.org/)

### Jakarta EE Runtimes on Github
* [Wildfly](https://github.com/wildfly/wildfly)
* [Open Liberty](https://github.com/OpenLiberty/open-liberty)
* [Eclipse GlassFish](https://github.com/eclipse-ee4j/glassfish)
* [Payara Server](https://github.com/payara/Payara)
* [Apache TomEE](https://github.com/apache/tomee)
* [JSF Java Server Faces: Primefaces](https://github.com/primefaces/primefaces)

### Java and Jakarta EE
* [Jakarta EE 9.1](src/site/markdown/JARTKARTA_EE.md)
* [Java jdk and jvm](src/site/markdown/JAVA_JDK_AND_JVM.md)
* [Java Server Faces JSF](src/site/markdown/JSF_PRIMEFACES.md)

## Imprint
* [(c) 2023 Thomas Woehlke](https://github.com/thomaswoehlke)
* [This Document](https://jakarta-ee-petclinic.github.io/petclinic-jakartaee/)
* [github repository](https://github.com/Jakarta-EE-Petclinic/petclinic-jakartaee)
* [maven project reports](https://java.woehlke.org/jakartaee/petclinic-jakartaee)
