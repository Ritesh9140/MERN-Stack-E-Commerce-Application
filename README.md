# MERN Stack E-Commerce Application

## Overview
This is a full-featured E-Commerce web application built using the MERN (MongoDB, Express.js, React.js, Node.js) stack. The application provides a complete online shopping experience with user authentication, product management, shopping cart functionality, order processing, and payment integration.



## Features

### User Features
- User registration and authentication
- Browse products by categories
- Search functionality with filters
- Product details with images, descriptions, and reviews
- Shopping cart management
- Checkout process
- Order history and tracking
- Review and rating system
- User profile management

### Admin Features
- Comprehensive admin dashboard
- Product management (add, update, delete)
- Order management
- User management
- Category management
- Sales analytics and reporting

## Technology Stack

### Frontend
- React.js
- Redux for state management
- React Router for navigation
- Axios for API requests
- Material UI and Bootstrap for styling
- React Toastify for notifications

### Backend
- Node.js with Express.js
- MongoDB for database
- Mongoose ODM
- JWT for authentication
- Bcrypt for password hashing
- Multer for file uploads

### Payment Processing
- Integration with payment gateways

## Installation and Setup

### Prerequisites
- Node.js (v14 or later)
- MongoDB
- npm or yarn

### Steps to Run Locally

1. **Clone the repository**
   ```
   git clone https://github.com/Ritesh9140/MERN-Stack-E-Commerce-Application.git
   cd MERN-Stack-E-Commerce-Application
   ```

2. **Setup Environment Variables**
   Create a `.env` file in the root directory and add the following:
   ```
   NODE_ENV = development
   PORT = 5000
   MONGO_URI = your_mongodb_uri
   JWT_SECRET = your_jwt_secret
   PAYPAL_CLIENT_ID = your_paypal_client_id
   ```

3. **Install backend dependencies**
   ```
   npm install
   ```

4. **Install frontend dependencies**
   ```
   cd frontend
   npm install
   ```

5. **Run the application**
   ```
   # Run backend and frontend concurrently
   cd ..
   npm run dev
   
   # Run backend only
   npm run server
   
   # Run frontend only
   npm run client
   ```

6. **Seed the database (optional)**
   ```
   # Import data
   npm run data:import
   
   # Destroy data
   npm run data:destroy
   ```

7. **Access the application**
   - Frontend: http://localhost:3000
   - Backend API: http://localhost:5000/api

## Project Structure
```
MERN-Stack-E-Commerce-Application/
├── frontend/           # React application
│   ├── public/         # Static files
│   ├── src/            # Source files
│   │   ├── actions/    # Redux actions
│   │   ├── components/ # React components
│   │   ├── constants/  # Constants and config
│   │   ├── reducers/   # Redux reducers
│   │   └── screens/    # Main application screens
├── backend/            # Node.js and Express server
│   ├── config/         # Configuration files
│   ├── controllers/    # Request handlers
│   ├── middleware/     # Express middleware
│   ├── models/         # MongoDB schema models
│   └── routes/         # API routes
├── uploads/            # Uploaded files storage
├── package.json        # Project dependencies and scripts
└── .env                # Environment variables (not tracked by git)
```

## API Endpoints

### Products
- GET `/api/products` - Get all products
- GET `/api/products/:id` - Get a single product
- POST `/api/products` - Create a product (admin only)
- PUT `/api/products/:id` - Update a product (admin only)
- DELETE `/api/products/:id` - Delete a product (admin only)
- POST `/api/products/:id/reviews` - Create a product review

### Users
- POST `/api/users/login` - Auth user & get token
- POST `/api/users` - Register a new user
- GET `/api/users/profile` - Get user profile
- PUT `/api/users/profile` - Update user profile
- GET `/api/users` - Get all users (admin only)
- DELETE `/api/users/:id` - Delete user (admin only)
- GET `/api/users/:id` - Get user by ID (admin only)
- PUT `/api/users/:id` - Update user (admin only)

### Orders
- POST `/api/orders` - Create new order
- GET `/api/orders/:id` - Get order by ID
- PUT `/api/orders/:id/pay` - Update order to paid
- PUT `/api/orders/:id/deliver` - Update order to delivered (admin only)
- GET `/api/orders/myorders` - Get logged in user orders
- GET `/api/orders` - Get all orders (admin only)

## UI Screenshots
![Dashboard](https://example.com/dashboard.png)
![Product Page](https://example.com/product-page.png)
![Cart](https://example.com/cart.png)

## Deployment
The application can be deployed using platforms like:
- Heroku
- Netlify (Frontend)
- MongoDB Atlas (Database)
- AWS

## Contributing
Contributions are welcome! Please feel free to submit a Pull Request.

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## License
This project is licensed under the MIT License - see the LICENSE file for details.

## Acknowledgments
- Thanks to all contributors who have helped make this project better
- Special thanks to the MERN stack community for the excellent documentation and resources

## Contact
Ritesh - [@Ritesh9140](https://github.com/Ritesh9140)

Project Link: [https://github.com/Ritesh9140/MERN-Stack-E-Commerce-Application](https://github.com/Ritesh9140/MERN-Stack-E-Commerce-Application)
