# 🍕 Romato – Food Delivery Web Application

A full-stack food delivery web application built using the MERN stack. Users can browse food items, add items to their cart, place orders, and make payments through Stripe Sandbox. An admin panel allows administrators to manage food items and orders.

## 🚀 Features

### Customer

* Browse available food items.
* View food descriptions and prices.
* Add or remove items from the shopping cart.
* Register and log in to an account.
* Enter delivery information.
* Proceed to checkout and test payments using Stripe Sandbox.
* View order history and order status.

### Admin

* Add new food items.
* View available food items.
* Remove food items.
* View customer orders.
* Update order processing status.

## 🛠️ Tech Stack

| Technology            | Purpose                     |
| --------------------- | --------------------------- |
| React.js              | Frontend user interface     |
| Vite                  | Frontend development server |
| Node.js               | Backend runtime             |
| Express.js            | Backend API                 |
| MongoDB               | Database                    |
| Mongoose              | MongoDB object modelling    |
| JWT                   | Authentication              |
| bcrypt                | Password hashing            |
| Stripe                | Sandbox payment integration |
| Axios                 | HTTP requests               |
| HTML, CSS, JavaScript | Web development             |

## 📁 Project Structure

```text
romato_delivery/
├── frontend/       # Customer-facing application
├── backend/        # Express APIs and database logic
├── admin/          # Admin dashboard
└── README.md
```

## ⚙️ Prerequisites

Install the following before running the project:

* Node.js and npm
* MongoDB Community Server
* Git (optional, for cloning the repository)

## 💻 Installation and Setup

### 1. Clone the repository

```bash
git clone https://github.com/jashwanthsai678/romato_delivery.git
cd romato_delivery
```

### 2. Configure the backend

```bash
cd backend
npm install
```

Create a `.env` file inside the `backend` directory. Add the required configuration variables using the names expected by the backend source code.

Typical variables include:

```env
MONGODB_URI=mongodb://localhost:27017/food_delivery
JWT_SECRET=your_jwt_secret
STRIPE_SECRET_KEY=your_stripe_test_secret_key
```

**Important:** These are example variable names. Verify the exact names used in the project's backend code and existing environment configuration before using them.

### 3. Start the backend

```bash
npm run server
```

The backend runs at:

`http://localhost:4000`

### 4. Start the customer frontend

Open a new terminal from the project root:

```bash
cd frontend
npm install
npm run dev
```

Open the local URL displayed by Vite, typically:

`http://localhost:5173`

### 5. Start the admin panel

Open another terminal:

```bash
cd admin
npm install
npm run dev
```

Open the local URL displayed by Vite. If port 5173 is already occupied, Vite may select another port, such as 5174.

## 💳 Payment Testing

The application integrates Stripe for payment processing.

* Use Stripe test-mode credentials for local testing.
* Use Stripe's official test card details only in Sandbox/test mode.
* Do not use real card details for testing.
* Never commit secret API keys or `.env` files to GitHub.

## 🧪 Testing Checklist

* [ ] Backend starts successfully.
* [ ] MongoDB connects successfully.
* [ ] Customer registration and login work.
* [ ] Food items appear on the homepage.
* [ ] Admin can add and remove food items.
* [ ] Items can be added to and removed from the cart.
* [ ] Delivery information can be submitted.
* [ ] Stripe Sandbox payment succeeds.
* [ ] Orders appear in My Orders.
* [ ] Orders appear in the admin panel.
* [ ] Admin can update order status.
* [ ] Track Order functionality is verified separately.

## 🔐 Security Notes

* Keep `.env` files and API keys private.
* Configure appropriate environment variables for local development and deployment.
* Never expose Stripe secret keys in frontend code.
* Use test credentials during development.

## 👨‍💻 Project Type

**Full-Stack Web Development | MERN Stack | Food Delivery Application**

This project demonstrates frontend development, REST API integration, database operations, authentication, cart management, order processing, admin functionality, and payment integration.

## 📄 Credits

Developed collaboratively. Refer to the original repository and contributors for project ownership and attribution.
