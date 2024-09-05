# Authify

Authify is a personal website with user authentication and basic profile management. This project demonstrates secure login and registration using JSON Web Tokens (JWT), CRUD operations, and basic PostgreSQL database management. The system is designed with scalability in mind, making use of RESTful API principles.

## Features

- **User Authentication**: Secure login and registration using JWT and password encryption with bcrypt.
- **CRUD Operations**: Users can create, read, update, and delete profile information.
- **Database Management**: PostgreSQL setup for user data management.
- **RESTful API**: The backend follows RESTful API principles for scalability.
  
## Tech Stack

- **Frontend**: JavaScript, HTML, CSS
- **Backend**: Node.js, Express.js
- **Database**: PostgreSQL
- **Authentication**: JWT, bcrypt

## Setup Instructions

### Prerequisites

- Node.js installed
- PostgreSQL installed

### Steps

1. Clone the repository:

    ```bash
    git clone https://github.com/yourusername/Authify.git
    cd Authify
    ```

2. Install dependencies:

    ```bash
    npm install
    ```

3. Set up PostgreSQL database:
    - Create a new PostgreSQL database for the project.
    - Update the `.env` file with your database credentials.

4. Create a `.env` file with the following content:

    ```env
    DATABASE_URL=postgres://username:password@localhost:5432/database_name
    JWT_SECRET=your_secret_key
    ```

5. Run migrations to set up your database schema (if using a migration tool like Knex.js).

6. Start the development server:

    ```bash
    npm start
    ```

7. Access the app at `http://localhost:3000`.

## Folder Structure

├── /controllers # Application logic and controllers 
├── /models # Database models and queries 
├── /routes # API routes 
├── /views # Frontend HTML and templates 
├── /middleware # Authentication and validation middleware 
├── /config # Database and JWT configurations 
├── .env # Environment variables 
└── README.md # Project documentation


## Future Improvements

- Add role-based authorization.
- Add email verification for new users.
- Implement unit and integration tests.

## License

This project is licensed under the MIT License.
