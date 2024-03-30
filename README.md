# NestboxesRungstedlund

## Background

Rungstedlund is a small nature park in Rungsted on the east coast of Zealand. The park belongs to the museum og Karen Blixen, and has been under protection since the 1960's.

In the park over 100 nestboxes is located. For many years, these nestboxes has been studied by registrering their content and ringing the chicks. A map of the nestboxes can be seen [here](Fuglereservatet_redekasser.pdf)

However, it is a logistical nightmare to know when to check a box, since it depends on whatever was in the box last.

## Purpose

To have a simple registration system of the content of a box, and to know which boxes to check next depending on their previous content.

## Methodology

A server database will hold the content of all data.

A front-end system will allow the user to make observations to the database. 

Using the data in the database, a list can be shown that depicts which boxes to check next.

## Documentation

### Frontend

Test-server: test.birdware.dk

### Rest API

First version found [here](./REST_API.md). 

Latest Test version is found [here](http://95.217.6.20/rungstedlund/swagger-ui)

### Backend

#### Server 

Test-server: 95.217.6.20
Owner: asktheo
TLS: *TODO*

#### Softwarestack

    Rest documentation                : Swagger-UI
    Web server                        : nginx with two way proxy for url
    Application server                : Embedded Tomcat with a single war-file on port : ****
    Settings for Spring application   : application.properties
    Rest controller and application   : Java (17) Spring
    Database                          : Database ******** in Mongo DB instance on port : *****
    Data collections                  : nestbox, status, record
    Mongo DB repository controller    : Java (17) Spring

## Acknowledgements

Backend built with XCode, Java 17, Mongo DB v. 4.4.25, IntelliJ IDEA CE by [asktheo](https://github.com/asktheo)
    


