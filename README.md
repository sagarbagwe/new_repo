
---
[ER model.pdf](https://github.com/sagarbagwe/new_repo/files/13715924/ER.model.pdf)

# Yoga Class Registration App

## Overview

This is a web application for managing yoga class registrations. It includes a user-friendly interface for submitting admission forms, viewing class schedules, and updating batch preferences. The application is built using the MERN stack (MongoDB, Express.js, React.js, Node.js) and uses MySQL for database storage.

## Features

- **Admission Form Submission:**
  - Users can fill out an admission form providing their name, age, and preferred batch timings.
  - Server-side validation ensures the integrity of the submitted data.

- **Batch Management:**
  - Users can view and select different yoga class batches based on timings.
  - The application ensures that users within the same month are assigned to the same batch.

- **Database Integration:**
  - MySQL is used as the database to store user information.
  - The server interacts with the database for form submissions, batch updates, and user queries.

- **Payment Processing (Mock):**
  - A mock payment function is included in the server logic to simulate payment processing.

## Project Structure

- **`client/`:** Contains the React.js frontend code.
- **`server/`:** Includes the Node.js/Express.js backend code.
- **`database/`:** Holds the SQL script for setting up the MySQL database.

## Getting Started

### Prerequisites

- Node.js and npm installed
- MySQL installed and running

### Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/your-username/yoga-class-registration.git
   ```

2. Navigate to the client directory:

   ```bash
   cd client
   ```

3. Install client dependencies:

   ```bash
   npm install
   ```

4. Navigate to the server directory:

   ```bash
   cd ../server
   ```

5. Install server dependencies:

   ```bash
   npm install
   ```

6. Create a MySQL database and run the SQL script in the `database/` folder to set up the necessary tables.

7. Set up environment variables by creating a `.env` file in the `server/` directory:

   ```env
   DB_HOST=localhost
   DB_USER=root
   DB_PASSWORD=your-mysql-password
   DB_DATABASE=yoga_classes
   DB_WAIT_FOR_CONNECTIONS=true
   DB_CONNECTION_LIMIT=10
   DB_QUEUE_LIMIT=0
   ```

8. Start the client and server:

   ```bash
   # In the client directory
   npm  run dev

   # In the server directory
   node server.js
   ```

9. Open the application in your browser: http://localhost:3000

