# Eureka Server

A minimal Spring Boot microservice acting as a service registry for the fitness application ecosystem.

## Features
- Service discovery and registration for microservices
- High availability and resilience (when clustered)
- Simple integration with Spring Cloud clients

## Main Endpoints
- `/eureka` — Eureka dashboard and REST endpoints for service registration/discovery

## Main Class
- `EurekaServerApplication` — Main entry point

## Configuration
- Main config: `src/main/resources/application.yaml`
- Default port: 8761 (can be changed in config)

## Build & Run
```sh
./gradlew build
./gradlew bootRun
```

## Usage
- Start this server before other microservices
- Other services should register themselves with this Eureka server for discovery
