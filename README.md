# 📊 Management Panel API

The **Management Panel API** is a web application designed for **Performanz R&D and Software Company**. The purpose of this project is to enable employees to manage and track product stock information, interview records, details of dispatched products, and reasons for the failure of discarded products. The application is built using **ASP.Net Core Multi-layer architecture** with **Entity Framework Core (EF Core)** as the ORM tool.

---

## 🛠️ Architecture Overview

### **Layered Architecture**
1. **Core Layer**:
   - The foundation layer of the project.
   - Contains:
     - **Models**: Represent the database entities.
     - **DTO Objects**: Data Transfer Objects for communication.
     - **Interfaces**: Contracts for repository, service, and UnitOfWork design patterns.
   - This layer defines the abstractions used by other layers.

2. **Repository Layer**:
   - Handles database operations.
   - Includes:
     - **Migrations**: To manage schema changes and apply them to the database.
     - **Seed Data**: Ensures default data is inserted during the initial migration.
   - Implements the **Repository Design Pattern**.

3. **Service Layer**:
   - Contains business logic and application services.
   - Includes:
     - **Mapping**: Maps entities to DTOs using the **AutoMapper** library.
     - **Validation**: Ensures data integrity.
     - **Exception Handling**: Manages application-specific exceptions.
   - Implements the **UnitOfWork Design Pattern**.

4. **API Layer**:
   - Exposes RESTful endpoints for the web application.
   - Directly communicates with the **Service Layer** to fulfill client requests.

---

## 🧩 Key Features

- **🔐 Authentication and Authorization**:
  - Secure login for employees.
  - Role-based access to resources.

- **📦 Stock Management**:
  - Track product stocks.
  - Manage inventory changes.

- **📋 Interview Management**:
  - Record and track interviewee details.

- **🚚 Product Tracking**:
  - Monitor dispatched products.
  - Record reasons for failed or discarded products.

- **📂 Multi-layered Design**:
  - Core, Repository, and Service layers ensure clean architecture and separation of concerns.

- **🔄 Database Integration**:
  - Built with EF Core for seamless database interaction.
  - Migrations for schema updates.

---

## 🚀 Technologies Used

- **Framework**: ASP.Net Core
- **ORM Tool**: Entity Framework Core (EF Core)
- **Mapping**: AutoMapper Library
- **Design Patterns**:
  - Repository Pattern
  - UnitOfWork Pattern
- **Database**: SQL Server
- **Language**: C#
- **API Testing**: Postman

---

## 🛠️ Installation & Setup

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/Sarizeybekk/ManagementPanelApi.git
   cd ManagementPanelApi

![image](https://user-images.githubusercontent.com/85437211/196987703-c3335166-b834-4746-8763-99c0ec6f0562.png)
