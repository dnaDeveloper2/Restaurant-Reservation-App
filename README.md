# Capstone: Restaurant Reservation System
## Overview
As a full stack developer at Periodic Tables, a startup focused on fine dining experiences, you've been entrusted with the development of a reservation system for fine dining restaurants. This system, designed for internal use by restaurant personnel, streamlines the reservation process, ensuring a seamless experience for both staff and patrons. The system's capabilities range from creating and managing reservations to assigning tables and maintaining the restaurant's operational flow.
![Screen Shot 2024-01-28 at 10 57 06 PM](https://github.com/dnaDeveloper2/Restaurant-Reservation-App/assets/130073814/69c5e9bb-dede-4566-8a08-b1cca74baced)




## Repository Structure
The repository is organized as a monorepo, hosting both frontend and backend projects, allowing for simultaneous development and testing. The backend operates on localhost:5001, handling database interactions and API requests, while the frontend, running on localhost:3000, presents an intuitive interface for the restaurant staff.

## Backend Structure
Knexfile.js: Configuration file for Knex, connecting to the PostgreSQL database.
Src/app.js: Main Express application, integrating routers.
Src/db/migrations: Knex migrations for database schema management.
Src/db/seeds/: Knex seeds for pre-populating the database with initial data.
Src/reservations/: Controllers and routers for reservation management.
Src/server.js: Node.js server setup.
Test/: Integration tests to ensure backend reliability.

## Frontend Structure
Src/App.js: Root React application component.
Src/dashboard/Dashboard.js: Main dashboard interface for managing reservations and tables.
Src/layout/: Core layout components, including navigation and error handling.
Src/utils/: Utility functions for API interactions and date-time manipulations.

## Installation and Setup
Repository Setup: Fork and clone the repository.
Environment Configuration:
Backend: Copy .env.sample to .env and configure your PostgreSQL database connection URLs.
Frontend: Copy .front-end/.env.sample to .front-end/.env. Adjustments are usually not needed unless the backend location changes.
Dependency Installation: Run npm install to install all necessary project dependencies.
Development Server: Launch the development server using npm run start:dev.

## Testing
The application includes a comprehensive suite of tests (unit, integration, and end-to-end) to ensure each component functions as expected.

Running Specific Tests: Use npm run test:X where X is the user story number.
Running All Tests: After completing all user stories, use npm test to execute all tests.

## Deployment
While the user stories don't explicitly cover deployment, it's advisable to adopt a continuous deployment approach, potentially using platforms like Render for hosting the application.

## Key Features and User Stories
The system's development is guided by a series of user stories, each focusing on a specific functionality, such as creating reservations, managing tables, and ensuring business rules (e.g., reservation times, table capacities) are adhered to.

## Example User Stories:
US-01 Create and list reservations: Manage new reservations and display them on the dashboard.
US-04 Seat reservation: Assign customers to tables and manage table occupancy.
US-06 Reservation Status: Track and update the status of each reservation.

## Contributing
This project is a significant step towards digitizing the reservation management process for fine dining establishments. Contributions and suggestions are welcome to enhance its functionality and user experience. Please note that direct pull requests to the main repository are not accepted; instead, fork the repository and submit your contributions for review.

Thank you for being part of this journey to streamline restaurant reservation management. Your expertise and dedication are crucial in making Periodic Tables a robust and user-friendly system for fine dining establishments.
