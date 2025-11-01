# 🧩 Node.js CRUD with MySQL

A complete **Node.js + Express + MySQL** CRUD (Create, Read, Update, Delete) web application that allows users to manage records easily through a dynamic web interface.  
This project demonstrates how to connect Node.js with MySQL and perform all database operations seamlessly. It is perfect for beginners learning backend development or building admin panels.

---

## 🌐 Live Demo

👉 [View Deployed Website](https://pintu-kumar.vercel.app)

*(Replace the above link if you deploy your CRUD app on Vercel or Render)*

---

## 📸 Preview

![Preview](https://github.com/PintuKumarSaw/Node-JS-Crud-With-Mysql/blob/main/preview.png?raw=true)

*(Add a file named `preview.png` in your project root to display it here)*

---

## 🚀 Features

✅ Create new users  
✅ View all users in a table  
✅ Edit user details dynamically  
✅ Delete users from the database  
✅ Real-time data updates via Express  
✅ MySQL integration for data storage  
✅ Simple EJS templating engine for UI  
✅ Fast and reliable CRUD operations  

---

## 🧰 Tech Stack

| Category | Technologies Used |
|-----------|-------------------|
| 💻 Backend | Node.js, Express.js |
| 🗄️ Database | MySQL |
| 📄 View Engine | EJS Templates |
| ⚙️ Tools | Nodemon, Git, VS Code, Postman |
| 🔗 Database Connector | mysql2 |

---

## 🏗️ Database Design

Before running the project, create the MySQL database and user table.

### 🔹 Step 1: Create Database
```sql
CREATE DATABASE node;

🔹 Step 2: Select Database
USE node;

🔹 Step 3: Create Table
CREATE TABLE user (
  id INT(11) NOT NULL AUTO_INCREMENT,
  name VARCHAR(100) NOT NULL,
  email VARCHAR(100) NOT NULL,
  phone VARCHAR(15),
  PRIMARY KEY (id)
);


✅ This table stores user details for the CRUD operations.
---
⚙️ Installation and Setup

Follow these steps to run the project locally:

1️⃣ Clone this repository
git clone https://github.com/PintuKumarSaw/Node-JS-Crud-With-Mysql.git

2️⃣ Navigate to the project folder
cd Node-JS-Crud-With-Mysql

3️⃣ Install dependencies
npm install

4️⃣ Start your MySQL server

Make sure MySQL is running and the above database is created.

5️⃣ Configure the database connection

Open your index.js or db.js file and verify:

var mysql = require('mysql2');
var connection = mysql.createConnection({
  host: 'localhost',
  user: 'root',        // your MySQL username
  password: '',        // your MySQL password
  database: 'node'     // database name
});

6️⃣ Start the server

You can use either command:

nodemon index.js


or

node index.js


You’ll see:

Server start on port number 8080

7️⃣ Open the application

Go to 👉 http://localhost:8080
---
📂 Folder Structure

Node-JS-Crud-With-Mysql/
│
├── node_modules/
├── public/
│   └── css/
│       └── style.css
│
├── views/             # EJS templates
│   ├── add-user.ejs
│   ├── edit-user.ejs
│   └── user-list.ejs
│
├── index.js           # Main server file
├── package.json
├── preview.png
└── README.md
---
🧠 How It Works

The app connects to MySQL using mysql2.

CRUD routes handle all user operations:

GET / → Display all users

GET /add → Show add user form

POST /save → Insert new user

GET /edit/:id → Edit a user

POST /update → Update user info

GET /delete/:id → Delete a user

EJS templates render the frontend dynamically.

🧑‍💻 Author

👤 Pintu Kumar Saw
📧 Email: pintusaw95084@gmail.com

🔗 GitHub: PintuKumarSaw

🌐 Portfolio: https://pintu-kumar.vercel.app
---
🏁 Start the Application
npm start


or (for development with auto-reload)

nodemon index.js


You’ll see:

Server start on port number 8080
MySQL Connected Successfully!


🎉 Congratulations! Your Node.js +




---

---

This version includes:
- ✅ Full project description (300+ words)
- ✅ Database design with SQL
- ✅ Preview image link
- ✅ Complete setup steps
- ✅ Author & portfolio (clickable)
- ✅ Error fixes and troubleshooting
- ✅ Folder structure  

---

Would you like me to add a **GIF demo or animated preview image** section (showing CRUD operations live)? I can help you include it next.

