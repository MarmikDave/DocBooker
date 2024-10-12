# Doctors Appointment Booking App

## Overview

This is a full-stack Doctors Appointment Booking application built using the MERN (MongoDB, Express, React, Node.js) stack. The application integrates **Razorpay** for payment processing and **Cloudinary** for image storage. It also features an admin panel for managing appointments and users.

## Features

- User registration and authentication
- Appointment booking and management
- Payment processing via **Razorpay**
- Image uploads and storage using **Cloudinary**
- Admin panel for managing appointments and users
- Client dashboard for users to view and manage their appointments
- Responsive design using **Tailwind CSS**

## Technologies Used

- **Frontend**: React, Vite, **Tailwind CSS**
- **Backend**: Node.js, Express
- **Database**: MongoDB
- **Payment Gateway**: **Razorpay**
- **Image Storage**: **Cloudinary**
- **File Upload**: Multer
- **Environment Variables**: dotenv

## Installation

### Prerequisites

- Node.js (v14 or higher)
- MongoDB (local or cloud instance)
- A **Razorpay** account for payment processing
- A **Cloudinary** account for image storage

### Clone the Repository

```bash
git clone https://github.com/MarmikDave/DocBooker.git
cd your-repo-name
````

### Server Setup

1. Navigate to the server directory:

   ```bash
   cd server
   ```

2. Install dependencies:

   ```bash
   npm install
   ```

3. Create a `.env` file in the `server` directory and add the following environment variables:

   ```env
   CLOUDINARY_NAME=your_cloudinary_name
   CLOUDINARY_API_KEY=your_cloudinary_api_key
   CLOUDINARY_API_SECRET=your_cloudinary_api_secret
   MONGO_URI=your_mongodb_uri
   ADMIN_EMAIL=your_admin_email
   ADMIN_PASSWORD=your_admin_password
   JWT_SECRET=your_jwt_secret
   RAZORPAY_API_KEY=your_razorpay_api_key
   RAZORPAY_SECRET=your_razorpay_secret
   CURRENCY=your_currency
   ```

4. Start the server:

   ```bash
   npm run server
   ```

### Client Setup

1. Navigate to the client directory:

   ```bash
   cd ../client
   ```

2. Install dependencies:

   ```bash
   npm install
   ```

3. Create a `.env` file in the `client` directory and add the following environment variable:

   ```env
   VITE_BACKEND_URI=http://localhost:5000
   ```

4. Start the client:

   ```bash
   npm run dev
   ```

### Admin Setup

1. Navigate to the admin directory (if separate, otherwise use the client directory):

   ```bash
   cd ../admin
   ```

2. Install dependencies (if separate):

   ```bash
   npm install
   ```

3. Create a `.env` file in the `admin` directory and add the same environment variables as the client:

   ```env
   VITE_BACKEND_URI=http://localhost:5000
   ```

## Usage

- Open your browser and navigate to the URL provided by Vite to access the application.
- Users can register, log in, and book appointments through the client dashboard.
- The client dashboard allows users to view and manage their appointments.
- Admins can manage appointments and users through the admin panel.
