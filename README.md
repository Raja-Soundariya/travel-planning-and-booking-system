# travel-planning-and-booking-system
## About the Project

The Travel Planning and Booking System is a web application developed using the MERN stack to simplify the process of searching, planning, and booking tour packages. It provides a user-friendly interface for customers to explore travel destinations, compare packages, make bookings, and complete online payments. An administrator can manage tour packages, bookings, users, and offers through a dedicated dashboard.

## Features

### Customer Features
- User registration and login
- Secure authentication using JSON Web Tokens (JWT)
- Browse available tour packages
- Search and filter packages by destination, price, and domestic or international category
- View detailed package information
- Book tour packages and enter traveller details
- Online payment integration using Razorpay
- View booking confirmation and status
- Forgot-password and password-reset functionality

### Admin Features
- Admin login and dashboard
- Add, update, and delete tour packages
- Manage customer bookings
- Manage users
- Manage special offers

## Technology Stack

**Frontend**
- React.js
- HTML5
- CSS3
- JavaScript
- React Router
- Axios

**Backend**
- Node.js
- Express.js
- REST APIs
- JWT Authentication
- bcrypt.js

**Database**
- MongoDB
- Mongoose

**External Services**
- Razorpay Payment Gateway
- Nodemailer for password recovery emails

**Development Tools**
- Visual Studio Code
- Git and GitHub
- MongoDB Compass
- Postman (for API testing)

## Project Structure

VIGNESH_TOURS_MERN/
│
├── backend/
│   ├── config/
│   │   └── db.js
│   │
│   ├── controllers/
│   │
│   ├── middleware/
│   │
│   ├── models/
│   │
│   ├── routes/
│   │   ├── adminRoutes.js
│   │   ├── authRoutes.js
│   │   ├── bookingRoutes.js
│   │   └── packageRoutes.js
│   │
│   ├── scripts/
│   │
│   ├── uploads/
│   │
│   ├── .env
│   ├── package.json
│   └── server.js
│
├── frontend/
│   ├── public/
│   │
│   ├── src/
│   │   ├── components/
│   │   ├── pages/
│   │   │   ├── user/
│   │   │   │   ├── Home.jsx
│   │   │   │   ├── Login.jsx
│   │   │   │   ├── Register.jsx
│   │   │   │   ├── Packages.jsx
│   │   │   │   ├── PackageDetails.jsx
│   │   │   │   ├── Booking.jsx
│   │   │   │   └── BookingSuccess.jsx
│   │   │   │
│   │   │   └── admin/
│   │   │       ├── AdminDashboard.jsx
│   │   │       ├── AddPackage.jsx
│   │   │       ├── EditPackage.jsx
│   │   │       ├── ManageOffers.jsx
│   │   │       └── ManageBookings.jsx
│   │   │
│   │   ├── services/
│   │   └── data/
│   │
│   ├── package.json
│   └── vite.config.js
│
├── README.md
└── .gitignore

*Note: The folder structure above is illustrative. Update it to match your actual project.*

## Prerequisites

Install the following before running the project:

- Node.js and npm
- MongoDB
- Git

## Installation and Setup

### 1. Clone the Repository

```bash
git clone YOUR_GITHUB_REPOSITORY_URL
cd travel-planning-and-booking-system
```

### 2. Set Up the Backend

```bash
cd backend
npm install
```

Create a `.env` file in the backend folder and configure the required environment variables according to your backend code.

Example variable names:

```env
PORT=5000
MONGO_URI=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret
```

Add any additional variables required by your implementation, such as email and Razorpay credentials. Never commit actual passwords, API secrets, or production credentials.

Start the backend:

```bash
npm run dev
```

### 3. Set Up the Frontend

Open a new terminal:

```bash
cd frontend
npm install
npm run dev
```

Open the local URL displayed in the terminal to access the application.

## Environment Configuration

Configure the necessary environment variables separately for the frontend and backend, based on the existing project configuration. Do not share real credentials in the repository.

## Security

- Authentication and role-based access control
- Password hashing
- Environment variables for sensitive configuration
- Payment verification through the payment integration

## Future Enhancements

- Enhanced travel recommendations
- Booking history and downloadable invoices
- Improved mobile responsiveness
- Additional payment and notification options

## Author

**Developed as an academic project.**

## License

This project is intended for educational purposes. Add a license if you intend to distribute or permit reuse of the source code.
