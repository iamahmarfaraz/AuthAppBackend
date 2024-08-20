**Project: Secure Authentication System with Node.js, Express.js, and MongoDB**

This project is a comprehensive backend application built using Node.js and Express.js, designed to implement a secure and scalable authentication system. Key features include:

**User Authentication and Authorization:-**
* Implemented login and signup functionalities with JSON Web Tokens (JWT) for session management and bcrypt for secure password hashing.
* Role-based access control (Student, Admin) enforced via middleware, ensuring that users only access authorized routes.
* Database Integration with MongoDB:
* Seamless connection to MongoDB using Mongoose, a powerful ORM for managing database interactions.
* Defined a robust User model schema to store user credentials and roles securely in the database.
* Middleware for Enhanced Functionality:
* Utilized middleware functions like cookie-parser and express.json to handle cookies and parse incoming JSON requests efficiently.
* Middleware also employed to verify JWT tokens and enforce role-based access control, securing the application’s endpoints.

**Project Structure:-**
* index.js: The central hub that initializes the Express app, sets up middleware, connects to MongoDB, and defines API routes.
* /config/database.js: Manages MongoDB connections using Mongoose, ensuring a stable and consistent database interaction.
* /routes/user.js: Houses routes for user-related actions such as login, signup, and protected operations, with integrated middleware for security checks.
* /models/User.js: Defines the User schema, laying the foundation for storing and retrieving user data in MongoDB.
* /middleware/auth.js: Contains critical middleware functions to authenticate JWTs and verify user roles, crucial for protecting sensitive routes.
* /controllers/Auth.js: Handles the business logic for authentication, processing login, and signup requests.

This project serves as a solid foundation for building secure, role-based authentication systems in modern web applications, leveraging the power of Node.js, Express.js, and MongoDB.
