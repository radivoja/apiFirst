# TransportCompany

A Spring Boot REST API for managing transport company operations, built using an API-first approach.

## Overview

TransportCompany is a backend application for managing core logistics and transport data.  
The system models transport-related business entities such as:

- Companies
- Drivers
- Trucks
- Shipments
- Goods

The project follows an **API-first design**, where the REST contract is defined in an OpenAPI specification and server-side code is generated from that definition.

## Features

- API-first development with OpenAPI
- CRUD operations for transport domain entities
- Search endpoints with filtering criteria
- PostgreSQL persistence
- Database versioning with Liquibase
- DTO mapping with MapStruct
- Spring Data JPA integration
- Swagger Codegen integration
- Lombok support for reduced boilerplate

## Domain Model

The application manages the following main entities:

- **Company** – basic company information such as name, location, and year founded
- **Driver** – driver details including experience and company association
- **Truck** – truck specifications such as manufacturer, model, horsepower, torque, fuel type, and cargo capacity
- **Shipment** – shipment data such as destination, distance, and loading date
- **Goods** – transported goods and quantity

Relationships between these entities are also reflected in the API model.

## Tech Stack

- Java 17
- Spring Boot 3
- Spring Web
- Spring Data JPA
- PostgreSQL
- Liquibase
- MapStruct
- Lombok
- OpenAPI / Swagger Codegen
- Maven
- WireMock (for testing)

## API-First Approach

This project uses an OpenAPI definition located in:

```bash
src/main/resources/transportCompany.yaml
