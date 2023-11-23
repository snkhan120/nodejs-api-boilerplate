# Node.js API Boilerplate

## Features

- Express.js for handling HTTP requests.
- MongoDB/Mongoose for database operations.
- JWT for authentication.
- Bcrypt for password hashing.
- Role-based access control.
- Error handling middleware.
- CORS handling.
- Sample User and Product models/controllers/routes.

## Getting Started

1. Clone the repository: `git clone https://github.com/your-username/nodejs-api-boilerplate.git`
2. Install dependencies: `npm install`
3. Set up your MongoDB connection in `config.js`.
4. Start the server: `npm start`

## API Endpoints

- **POST /api/auth/register** - Register a new user.
- **POST /api/auth/login** - Login and receive a JWT.
- **GET /api/users** - Get all users (requires authentication).
- **GET /api/products** - Get all products (public).
- **POST /api/products** - Create a new product (requires admin role).

## Project Structure

- **config.js**: Configuration file for database connection and other settings.
- **middlewares/auth.js**: Middleware for JWT authentication.
- **middlewares/roleMiddleware.js**: Middleware for role-based access control.
- **models/User.js**: User model with password hashing.
- **models/Product.js**: Sample Product model.
- **routes/authRoutes.js**: Authentication routes.
- **routes/userRoutes.js**: User-related routes.
- **routes/productRoutes.js**: Product-related routes.
- **controllers/authController.js**: Controller for authentication.
- **controllers/userController.js**: Controller for user-related actions.
- **controllers/productController.js**: Controller for product-related actions.

## Notes

- Make sure to customize the models, controllers, and routes based on your project's requirements.
- Update error handling to suit your application's needs.
- Add validation and error checking for production use.
