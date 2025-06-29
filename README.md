# PyS.eureka-service

[![PyS.eureka-service CI](https://github.com/PyS-services/PyS.eureka-service/actions/workflows/maven.yml/badge.svg?branch=main)](https://github.com/PyS-services/PyS.eureka-service/actions/workflows/maven.yml)

## Description

PyS.eureka-service is a Netflix Eureka Server implementation for service discovery in microservices architecture. It provides a REST-based service registry for locating services for load balancing and failover of middle-tier servers.

## Features

- Service registration and discovery
- High availability and fault tolerance
- RESTful API for service management
- Health monitoring and status reporting via Actuator
- Self-preservation mode for network issues
- Distributed tracing with OpenTelemetry
- Caching with Caffeine

## Prerequisites

- Java 24
- Maven 3.6+
- Docker (optional)

## Dependencies

- Spring Boot 3.5.3
- Spring Cloud 2025.0.0
- Spring Cloud Netflix Eureka Server
- OpenTelemetry Spring Boot Starter 2.17.0
- Caffeine Cache

## Getting Started

### Local Development

1. Clone the repository:
```bash
git clone https://github.com/PyS-services/PyS.eureka-service.git
cd PyS.eureka-service
```

2. Build the project:
```bash
./mvnw clean package
```

3. Run the application:
```bash
java -jar target/eureka-service-0.0.1-SNAPSHOT.jar
```

### Docker

Build and run using Docker:

```bash
# Build the image
docker build -t eureka-service .

# Run the container
docker run -p 8761:8761 eureka-service
```

## Configuration

The application can be configured through `application.yml` or environment variables:

```yaml
server:
  port: 8761

eureka:
  instance:
    hostname: localhost
  client:
    registerWithEureka: false
    fetchRegistry: false
```

## API Documentation

The Eureka Server provides a web interface at `http://localhost:8761` when running locally.

## Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Support

For support, please open an issue in the GitHub repository.
