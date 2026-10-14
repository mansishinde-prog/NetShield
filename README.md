# Intelligent Log Analytics and Threat Detection Engine (NetShield)

<p align="center">
  <strong>A SIEM-inspired cybersecurity monitoring application built with Java and Spring Boot.</strong>
</p>

<p align="center">
  <a href="https://netshield-production-9266.up.railway.app">Live Demo</a> |
  <a href="https://github.com/mansishinde-prog/NetShield">GitHub Repository</a>
</p>

## Overview

NetShield is a Java-based cybersecurity monitoring application designed to demonstrate application log analysis, security event monitoring, and rule-based threat detection.

The project uses Spring Boot and database integration to provide a foundation for collecting, processing, and presenting application security events through a web interface.

## Problem Statement

Modern applications generate large volumes of logs. Without appropriate monitoring, suspicious activity can be difficult to identify and investigate.

NetShield explores how log parsing, security rules, alert management, and dashboard visualizations can help improve security visibility.

## Key Features

Include and describe the features that are implemented and tested in the current version:

- **Log Analytics:** Process and inspect application log records.
- **Threat Detection:** Evaluate supported suspicious activity patterns using predefined rules.
- **Alert Management:** Record and display detected security events.
- **Dashboard:** Present available log and security information.
- **Database Integration:** Use Spring Data JPA and Hibernate for persistence.
- **User Authentication:** Provide application access through the configured authentication system.

## Threat Detection Concepts

The project is designed around SIEM-inspired detection concepts, including:

- Repeated failed login attempts
- SQL injection indicators
- Suspicious URL patterns
- High-frequency requests
- Repeated unauthorized access attempts

Detection coverage depends on the rules implemented in the current codebase.

## Technology Stack

### Backend
- Java
- Spring Boot
- Spring MVC

### Logging and Monitoring
- Log4j2
- Scheduled services, where implemented

### Database
- H2 Database
- Spring Data JPA
- Hibernate ORM

### Frontend
- Thymeleaf
- HTML
- CSS
- Bootstrap
- JavaScript

### Deployment
- Railway
- Maven

## System Architecture

Add your architecture diagram below after uploading it to the repository.

![System Architecture](images/hld.png)

## Dashboard Preview

Add a screenshot of your actual application dashboard at `images/dashboard.png`.

![NetShield Dashboard](images/dashboard.png)

## Project Structure

```text
NetShield/
├── images/
├── src/
│   └── main/
│       ├── java/com/loganalytics/
│       │   ├── model/
│       │   ├── repository/
│       │   ├── service/
│       │   ├── engine/
│       │   ├── controller/
│       │   ├── dto/
│       │   └── config/
│       └── resources/
│           ├── templates/
│           ├── static/
│           └── application.properties
├── pom.xml
├── README.md
├── LICENSE
└── .gitignore
```

## Getting Started

### Prerequisites

- Java Development Kit
- Maven
- Git

### Clone the Repository

```bash
git clone https://github.com/mansishinde-prog/NetShield.git
cd NetShield
```

### Run Locally

```bash
mvn spring-boot:run
```

Open the local address configured by your application. The current development configuration has used port `8000`:

http://localhost:8000

### Deployment

The application is deployed on Railway:

https://netshield-production-9266.up.railway.app

## Future Enhancements

- Machine-learning-based anomaly detection
- MITRE ATT&CK mapping
- Threat intelligence integration
- Geo-IP analysis
- Email security alerts
- Kafka-based log streaming
- Docker support
- Elasticsearch integration
- SOC case management

## Learning Outcomes

- Cybersecurity monitoring concepts
- SIEM fundamentals
- Java and Spring Boot development
- Log analysis and rule-based detection
- Database integration
- Web application deployment

## License

This project is available under the MIT License, subject to the terms of the repository's `LICENSE` file.