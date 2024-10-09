# **Budget Tracker - Full Stack Application**

---

## **Overview**

The **Budget Tracker** is a comprehensive full-stack web application built to help users manage multiple accounts and track their financial transactions in real-time. The app provides secure authentication, dynamic transaction management, and responsive user interfaces for an optimal experience on any device.

The system is designed with scalability and maintainability in mind, using a MERN (MongoDB, Express, React, Node.js) architecture. The backend is responsible for user authentication, account management, and transaction persistence, while the frontend offers a user-friendly interface for seamless interaction with the app’s features.

---

## **Tech Stack Overview**

### **Frontend**:
- **React.js**: A powerful JavaScript library for building user interfaces, offering fast rendering with a virtual DOM.
- **React Router**: Enables dynamic routing in the app for smooth navigation between different pages.
- **Axios**: A promise-based HTTP client used to communicate with the backend API.
- **CSS Modules**: Scoped and modularized styling for React components to avoid CSS conflicts and improve maintainability.

### **Backend**:
- **Node.js**: Handles server-side logic with an asynchronous, non-blocking model for efficient handling of requests.
- **Express.js**: A minimalist web framework for Node.js, used to create RESTful APIs for handling requests.
- **JWT Authentication**: JSON Web Tokens (JWT) for user authentication and session management.
- **Bcrypt.js**: For securely hashing and storing user passwords.

### **Database**:
- **MongoDB**: A NoSQL database designed for flexibility, scalability, and high performance. Stores user data, accounts, and transactions.
- **Mongoose**: ODM (Object Data Modeling) library for MongoDB and Node.js, used to manage schemas and data models.

### **Deployment**:
- **Netlify**: Hosting platform for the frontend, providing continuous deployment, CDN, and HTTPS out of the box.
- **Render**: Hosting platform for the backend with automatic deployments from the GitHub repository.

---

## **Features**

### **1. User Authentication**
- **JWT-based Authentication**: Secure login and registration system where user sessions are maintained via JSON Web Tokens.
- **Password Hashing**: User passwords are hashed using `bcrypt` before being stored in the database for added security.
  
### **2. Account Management**
- **Multiple Accounts**: Users can create multiple financial accounts, such as checking, savings, or investment accounts, under a single profile.
- **CRUD Operations**: Full Create, Read, Update, and Delete functionality for accounts, enabling users to manage their accounts effortlessly.

### **3. Transaction Management**
- **Add Transactions**: Users can log financial transactions such as income and expenses under different accounts.
- **Edit Transactions**: Users can update transaction details (amount, description, date).
- **Delete Transactions**: Users can remove any transaction from an account, with real-time updates.
  
### **4. Responsive Design**
- **Cross-Device Compatibility**: The app is fully responsive, ensuring a smooth experience on desktop, tablet, and mobile devices.
  
### **5. Persistent Data Storage**
- **MongoDB Atlas**: The app uses MongoDB Atlas for reliable and scalable cloud-based database storage.
  
---

## **Folder Structure**

```plaintext
Budget-Tracker-Full-Stack/
├── client/                     # Frontend React application
│   ├── public/                 # Public assets (HTML, icons, etc.)
│   ├── src/
│   │   ├── components/         # Reusable React components
│   │   ├── pages/              # Main app pages (Login, Dashboard, etc.)
│   │   ├── utils/              # Helper functions (API requests, etc.)
│   │   ├── App.js              # App component with routing
│   │   └── index.js            # Entry point for React app
│   └── package.json            # Frontend dependencies and scripts
├── server/                     # Backend Node.js application
│   ├── config/                 # Configuration files (DB connection, JWT secret)
│   ├── controllers/            # Controller logic for API endpoints
│   ├── middleware/             # Authentication and error handling middleware
│   ├── models/                 # Mongoose schemas (User, Account, Transaction)
│   ├── routes/                 # API route definitions (auth, accounts, transactions)
│   ├── server.js               # Main entry point for the Node.js server
│   └── package.json            # Backend dependencies and scripts
├── README.md                   # Project documentation
└── .gitignore                  # Files to ignore in version control


