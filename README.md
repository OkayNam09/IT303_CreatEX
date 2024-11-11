# IT303_CreatEX
Project Repository for ITEN08C (System Integration and Architecture)

### Project Overview
This project is an integrated system that leverages .NET MAUI to build both mobile and desktop applications with SQLite for local storage. Hosted on Azure, the backend supports essential mental health services for users and professionals, offering a seamless, cross-platform experience.

### Hardware Requirements

#### Desktop: 

|Hardware|	Minimum                                            |	Recommended            |
|:------:|:---------------------------------------------------:|:-----------------------:|
|CPU     |	Intel Core i3 or AMD equivalent (2.0GHz or higher) |	Intel Core i5 or better|
|RAM     |	4 GB	                                             |  8GB or higher          |
|Storage |	500 MB                                             |	1 GB                   |
|Internet|	Yes	                                               |  Yes                    |

#### Mobile:

|Hardware|	Minimum                                            |	Recommended            |
|:------:|:---------------------------------------------------:|:-----------------------:|
|CPU     |	1.4 GHz Quad-core                                  |	2.0 GHz Octa-core      |
|RAM     |	2 GB	                                             |  4GB or higher          |
|Storage |	32 GB                                              |	64 GB                  |
|Internet|	Yes	                                               |  Yes                    |


### Technology Stack
#### Frontend
- .NET MAUI: A cross-platform framework to create mobile and desktop applications from a single codebase.
- SQLite: Local database for offline access and fast data retrieval on client devices.

### Backend Services (Azure-hosted)
- Azure SQL Database: Centralized data storage for user and application data.
- Azure Cache for Redis: Caching layer for quicker data access.
- Azure Service Bus: Manages asynchronous communication between services.
- Microservices: Modularized backend services for key functions:
  - Profile Service: Manages user profiles.
  - Doctor Search Service: Searches for mental health professionals.
  - Appointment Service: Schedules and manages appointments.
  - Notification Service: Sends reminders and updates.
  - Authentication Service: Manages secure user login and access.

### Background Services
- Application Insights: Monitors app performance and logs issues.
- Serilog: Captures detailed logs for troubleshooting and analytics.

### System Architecture
The system is designed with three main layers:

1. #### Client Layer:
Mobile app (using .NET MAUI) and Desktop app (WinUI) with specific services and local storage (SQLite for mobile, SQL Server Express for desktop).

2. #### Backend Services Layer:
Includes modular microservices for core app functionality, managed via Azure API Management and Azure Load Balancer for optimized scalability and performance.

3. #### Data Layer:
Utilizes Azure SQL Database, Redis Cache, and Service Bus for reliable data storage, caching, and service communication.

### Project Team:
- **Blanza, Namron Spencer P.** (Project Leader/Lead Programmer)
- **Pabines, Kenneth T.**
- **Ramirez, Patricia Beatriz J.**
- **Ronsairo, Jozell A.**
