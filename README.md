# Microservices_Application_for_Booking_Tickets


## Overview
This project is a microservices-based application for booking tickets, deployed on Microsoft Azure using AKS.

## Microservices
- **User Service: Manages user information and authentication.
- **Booking Service:Handles booking operations.
- **Payment Service:Manages payment transactions.
- **Notification Service: Sends notifications upon successful bookings.

## Technologies
- Spring Boot
- Docker
- Kubernetes
- Azure Kubernetes Service (AKS)
- MySQL/PostgreSQL

## Setup Instructions

### Prerequisites
- Java 11
- Docker
- Kubernetes CLI
- Azure CLI

### Build and Push Docker Images

1. Build the Docker images:

```bash
cd user-service
mvn clean package
docker build -t <MyApplication>.azurecr.io/user-service:v1 .
docker push <MyApplication>.azurecr.io/user-service:v1
