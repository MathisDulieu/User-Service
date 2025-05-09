# User-Service

## Description
Comprehensive user management system for SUPMAP that handles profile administration, location tracking,
administrative controls, and usage analytics. Provides functionalities for user profile customization,
account lifecycle management, administrative dashboard data, user search capabilities, and real-time
location updates with performance metrics monitoring for system optimization.

## Features
- User profile management
- Navigation preferences (route options, default settings)
- User contribution tracking
- Profile image handling
- User statistics and activity tracking
- Community reputation management
- Privacy and data management

## Tech Stack
- Java 21
- Spring Boot 3.4.4
- MongoDB for user data storage
- Kafka for inter-service communication
- Prometheus for monitoring

## Dependencies
- shared-models: Common data models across SUPMAP services
- database-utils: Database utility functions
- Spring Boot Web for RESTful API endpoints
- MongoDB for data persistence
- Kafka for event messaging
- Prometheus for metrics collection

## Configuration
The service can be configured via environment variables:

```yaml
supmap:
  properties:
    app-email: your-app-email@example.com
    database-name: user_service_db
    elasticsearch-password: your-password
    elasticsearch-url: http://elasticsearch:9200
    elasticsearch-username: elastic
    kafka-bootstrap-servers: kafka:9092
    mail-modified-username: true
    mail-password: your-mail-password
    mongo-uri: mongodb://user:password@mongodb:27017/user_service_db