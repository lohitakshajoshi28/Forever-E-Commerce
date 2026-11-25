# 🛍️ Forever — Full-Stack E-Commerce Platform

A modern, full-stack clothing e-commerce web application featuring product discovery, user authentication, shopping cart management, online payments, and a dedicated admin dashboard.

**Forever** provides a complete online shopping experience with separate customer and administration interfaces, powered by a React frontend, Node.js backend, and MongoDB database.

---

## 🌟 Project Overview

Forever is a full-stack e-commerce platform designed to make online clothing shopping simple and convenient.

Customers can explore clothing collections, view product details, select sizes, manage their shopping carts, and place orders using integrated payment options.

The platform also includes an administration dashboard that allows administrators to manage products and monitor customer orders.

## ✨ Key Features

### 🛒 Customer Features

- User registration and login.
- Browse clothing collections.
- Product categorization and filtering.
- Product details and size selection.
- Search functionality.
- Add, update, and remove cart items.
- Secure user authentication using JWT.
- Order placement and order history.
- Responsive shopping interface.

### 💳 Payment Integration

- Stripe payment integration.
- Razorpay payment integration.
- Cash on Delivery (COD).
- Payment verification and order management.

### ⚙️ Admin Dashboard

- Dedicated admin login.
- Add new products.
- Upload product images.
- View available products.
- Remove existing products.
- View customer orders.
- Update order statuses.

### 📱 Responsive Design

- Responsive customer interface.
- Clean and modern shopping experience.
- Easy navigation across application pages.
- Mobile and desktop compatibility.

## 🛠️ Technology Stack

| Category | Technologies |
|---|---|
| Frontend | React.js, Vite |
| Styling | Tailwind CSS |
| Routing | React Router DOM |
| API Integration | Axios |
| Backend | Node.js, Express.js |
| Database | MongoDB, Mongoose |
| Authentication | JWT, bcrypt |
| Image Management | Cloudinary |
| Payments | Stripe, Razorpay, COD |
| Notifications | React Toastify |
| Version Control | Git, GitHub |

## 🏗️ Project Architecture

The application is divided into three major modules:

**1. Frontend**

The customer-facing application where users browse products, manage their carts, authenticate, and place orders.

**2. Backend**

The server-side application responsible for API requests, authentication, database operations, product management, cart functionality, and order processing.

**3. Admin Dashboard**

A separate interface for administrators to manage products and customer orders.

## 📂 Project Structure

```text
Forever-E-Commerce/
│
├── admin/
│   ├── src/
│   ├── public/
│   ├── package.json
│   └── vite.config.js
│
├── backend/
│   ├── config/
│   ├── controllers/
│   ├── middleware/
│   ├── models/
│   ├── routes/
│   ├── server.js
│   └── package.json
│
├── frontend/
│   ├── src/
│   │   ├── assets/
│   │   ├── components/
│   │   ├── context/
│   │   └── pages/
│   ├── public/
│   ├── package.json
│   └── vite.config.js
│
├── .gitignore
└── README.md
```

## ⚙️ Installation and Setup

Follow these instructions to run the project locally on your computer.

### Prerequisites

Make sure you have installed:

- Node.js and npm
- Git
- Visual Studio Code
- MongoDB database
- Cloudinary account

### Step 1: Clone the Repository

```bash
git clone https://github.com/lohitakshajoshi28/Forever-E-Commerce.git
```

### Step 2: Navigate to the Project

```bash
cd Forever-E-Commerce
```

### Step 3: Configure the Backend

Navigate to the backend folder:

```bash
cd backend
```

Install dependencies:

```bash
npm install
```

Create a `.env` file inside the backend folder.

Add the following environment variables:

```env
PORT=4000

MONGODB_URI=your_mongodb_connection_string

CLOUDINARY_NAME=your_cloudinary_name
CLOUDINARY_API_KEY=your_cloudinary_api_key
CLOUDINARY_SECRET_KEY=your_cloudinary_secret_key

JWT_SECRET=your_jwt_secret

ADMIN_EMAIL=your_admin_email
ADMIN_PASSWORD=your_admin_password

STRIPE_SECRET_KEY=your_stripe_secret_key

RAZORPAY_KEY_ID=your_razorpay_key_id
RAZORPAY_KEY_SECRET=your_razorpay_key_secret
```

Replace the placeholder values with your own credentials. Never upload real credentials to GitHub.

Start the backend:

```bash
npm run server
```

The backend will run on:

```text
http://localhost:4000
```

### Step 4: Configure the Frontend

Open a new terminal and navigate to the frontend:

```bash
cd frontend
```

Install dependencies:

```bash
npm install
```

Create a `.env` file inside the frontend folder:

```env
VITE_BACKEND_URL=http://localhost:4000
VITE_RAZORPAY_KEY_ID=your_razorpay_key_id
```

Start the frontend:

```bash
npm run dev
```

The frontend will generally run on:

```text
http://localhost:5173
```

### Step 5: Configure the Admin Dashboard

Open another terminal:

```bash
cd admin
```

Install dependencies:

```bash
npm install
```

Create a `.env` file inside the admin folder:

```env
VITE_BACKEND_URL=http://localhost:4000
```

Start the admin dashboard:

```bash
npm run dev
```

Vite will display the local admin URL in the terminal.

### Step 6: Access the Application

Once all three services are running:

| Application | Local Address |
|---|---|
| Customer Frontend | http://localhost:5173 |
| Backend API | http://localhost:4000 |
| Admin Dashboard | Check the Vite terminal output |

You should now be able to access the different parts of Forever locally.

## 🔄 Application Workflow

1. A customer visits the shopping website.
2. The frontend retrieves available products through backend APIs.
3. The customer registers or logs into their account.
4. Products can be selected and added to the shopping cart.
5. The customer enters delivery information and selects a payment method.
6. The backend processes the order and payment workflow.
7. Order information is stored in MongoDB.
8. Administrators can access the admin dashboard to manage products and orders.

## 🔐 Security and Configuration

The project uses:

- JWT-based authentication.
- Password hashing with bcrypt.
- Protected backend routes.
- Environment variables for sensitive configuration.
- Separate admin authentication.

**Important:** Keep `.env` files private and never commit API keys, database credentials, or payment secrets to a public repository.

## 🚀 Future Improvements

- Wishlist functionality.
- Product reviews and ratings.
- Advanced product recommendations.
- Improved admin analytics dashboard.
- Order tracking enhancements.
- Email notifications.
- Additional product filtering options.

## 👨‍💻 Author

**Lohitaksha Joshi**

GitHub: [@lohitakshajoshi28](https://github.com/lohitakshajoshi28)

Project Repository: [Forever-E-Commerce](https://github.com/lohitakshajoshi28/Forever-E-Commerce)

---

⭐ If you find this project interesting, consider giving the repository a star!

**Forever — Making Online Shopping Simple and Convenient.**
