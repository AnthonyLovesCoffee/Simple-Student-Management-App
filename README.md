# Simple-Student-Management-App

---

## **Overview**
This very basic student management app is a microservices-based application for managing student records. It demonstrates the integration of multiple technology stacks, including Flask, FastAPI, PostgreSQL, and Docker, to create a modular, scalable, and efficient system. The application features a basic interface to add and view student data, supported by APIs and secure database connectivity.

---

## **Features**
- **Web Application**: 
  - Flask-based frontend to interact with the system.
  - Endpoints to add (`/add`) and view (`/all`) student records.

- **API Service**:
  - FastAPI backend for processing requests and managing student data.
  - Swagger UI for API testing and interaction.

- **Database Service**:
  - PostgreSQL database for storing student records securely.
  - Adminer for visual database management.

- **Containerized Architecture**:
  - Docker and Docker Compose used to containerize services for scalability and simplified deployment.

---

## **Technologies Used**
- Python  
- Flask, FastAPI  
- PostgreSQL, Adminer
- Docker, Docker Compose  
- Git  

---

## **System Flow**
1. Users interact with the **Flask web app** to add or view student records.
2. Requests are sent to the **FastAPI backend**, which processes data.
3. The **PostgreSQL database** securely stores all student records.
4. Adminer provides a visual interface for database inspection and management.
5. Docker Compose ensures seamless communication between services within isolated networks.

---

## **Setup Instructions**
1. **Clone the Repository**:
   ```bash
   git clone AnthonyLovesCoffee/Simple-Student-Management-App
   cd Simple-Student-Management-App
   ```

2. **Set Up Environment Variables**:
   - Create a `.env` file in the root directory to store PostgreSQL credentials:
     ```
     POSTGRES_DB=x
     POSTGRES_USER=y
     POSTGRES_PASSWORD=z
     ```

3. **Build and Run the Application**:
   - Start all services with Docker Compose:
     ```bash
     docker-compose up --build
     ```
   - Access the web app at [http://127.0.0.1:8090](http://127.0.0.1:8090).
   - Use Adminer at [http://127.0.0.1:8091](http://127.0.0.1:8091) to manage the database.

4. **Test the Application**:
   - Visit [http://127.0.0.1:8090/add](http://127.0.0.1:8090/add) to add student records.
   - Visit [http://127.0.0.1:8090/all](http://127.0.0.1:8090/all) to view all records.

---