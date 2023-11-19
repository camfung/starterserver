# Express and Passport.js Application

This application is an Express server integrated with Passport.js for authentication, using a PostgreSQL database. It follows best practices in code organization and structure.

## Features

- **Express Server**: A robust framework for creating server-side applications and APIs.
- **Passport.js Integration**: For handling user authentication with support for multiple strategies.
- **PostgreSQL Database**: Using `pg` to connect to a PostgreSQL database for data persistence.
- **Modular Structure**: Organized codebase with separate directories for routes, controllers, models (DAO), and middleware.
- **Environment Variable Management**: Using `.env` for storing sensitive configuration data.
- **Session Management**: Using `express-session` for handling user sessions.

## Project Structure

- `index.js`: The entry point of the application, setting up the server and middleware.
- `config.js`: Configuration file to manage environment variables.
- `dao/`: Data Access Object folder containing:
  - `db.js`: Manages the database connection and provides a query execution function.
- `controllers/`: Contains files for route handlers grouped by functionality.
  - `index.js`: Aggregates all controller routes and exports them for use in the main application file.
- `middlewares/`: Contains middleware configurations, including:
  - `passport.js`: Configuration for Passport.js authentication strategies and session serialization/deserialization.
- `.env`: (Not tracked by Git) Contains environment variables such as database connection details and session secret.
- `.gitignore`: Specifies intentionally untracked files to ignore by Git.

## Setup and Installation

1. **Install Dependencies**:
   ```bash
   npm install
   ```
