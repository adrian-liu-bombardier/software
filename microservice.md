# Microservice

## Why Microservice?

Because of several drawbacks of previous architecture - Monolithic Architecture:

1. Unreliable: 

![](.gitbook/assets/image%20%284%29.png)

if part of service is down, entire services are down. impact the availability of entire application

2. Unsalable: there is a need that we need to scale up, such as some services are cpu intensive and some are memory intensive. With microservice, we are able to only scale up the services that needs scale up independently. 

3. Slow deployment: every time adds a new feature or change the service, Monolithic need to redeploy from scratch, microservice only needs to deploy partial, which is faster

4. Large & complex application: if the service is down, developers have to start from zero to look up the bugs

## What is Microservice?

![](.gitbook/assets/image%20%287%29.png)

Each component implement single business capability

They will communicate through APIs

### Example:

![](.gitbook/assets/image%20%2815%29.png)



![](.gitbook/assets/image%20%281%29.png)



They are independent to each other, their libraries are different, database are different

API Gateway: forward the request from clients to the corresponding services 

## Features of Microservice Architecture

![](.gitbook/assets/image%20%2812%29.png)



1. for simplicity 
2. independent
3. written in any languages
4. each microservice does not need to understand the implementation of other microservices

## Advantages

![](.gitbook/assets/image%20%2819%29.png)







