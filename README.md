# Springboot-angular
This is a simple User Management application built using **Spring Boot** (Java) for the backend and **Angular** for the frontend. The application allows you to list users and add new users.

## Features

- List all users
- Add new users
- Responsive UI with basic navigation

## Prerequisites

Before you can run the application, make sure you have the following installed:

- **Java** 
- **Maven** (for building the Spring Boot application)
- **Node.js** and **npm** (for running the Angular frontend)
- **Angular CLI** (to create and manage Angular projects)

## Backend Setup (Spring Boot)

The backend is a **Spring Boot** application using **Spring Data JPA** to manage users in an in-memory MySql database (or you can configure a different database such as MySQL).

### Steps to Run the Backend

The backend server will start at http://localhost:8080.
Available Backend Endpoints
GET /api/v1/users - Retrieves the list of users
POST /api/v1/users - Adds a new user

Frontend Setup (Angular)

The frontend is built using Angular, which provides a user-friendly interface for interacting with the backend. You can view a list of users and add new users through the frontend.

Steps to Run the Frontend
1.Navigate to the in your terminal.

2.Install the necessary dependencies by running:
npm install -g @angular/cli
ng new task1-frontend --no-standalone
cd task1-frontend
npm install bootstrap

3.Start the Angular development server:
ng serve

The frontend application will start at http://localhost:4200.

Features
User List: Displays all users in a table format.
Add User: Form to add new users to the system.

Angular Components
UserListComponent(ng g c user-list): Displays the list of users.
CreateUserComponent(ng g c create-user): Allows you to add a new user via a form.
UserService(ng g s user): Handles HTTP requests to the Spring Boot backend.

Running Both Applications Together
Once both the backend and frontend servers are running:

Navigate to http://localhost:4200 to interact with the frontend.
The frontend will interact with the backend at http://localhost:8080/api/v1/users for ma
