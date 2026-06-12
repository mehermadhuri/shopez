\# ShopEz - E-Commerce Application



A full stack e-commerce application built with MERN Stack.



\## Tech Stack

\- Frontend: React.js

\- Backend: Node.js, Express.js

\- Database: MongoDB Atlas



\---



\## 1. TECHNICAL ARCHITECTURE



Client (React) → REST API → Server (Express/Node) → MongoDB Atlas



\- Frontend runs on port 3000

\- Backend runs on port 5000

\- Database hosted on MongoDB Atlas Cloud



\---



\## 2. ER DIAGRAM



Users Collection:

\- \_id, name, email, password, isAdmin, createdAt



Products Collection:

\- \_id, name, price, description, image, category, stock, createdAt



Orders Collection (future):

\- \_id, user (ref: Users), products, totalPrice, status, createdAt



\---



\## 3. FEATURES



\- User Registration and Login

\- Browse Products

\- Add to Cart

\- Secure Authentication using JWT

\- Admin can manage products

\- Responsive UI



\---



\## 4. ROLES AND RESPONSIBILITIES



Customer:

\- Register/Login

\- Browse and search products

\- Add to cart and checkout



Admin:

\- Add/Edit/Delete products

\- View all orders

\- Manage users



\---



\## 5. USER FLOW



1\. User visits ShopEz → Home Page

2\. User clicks Register → fills form → account created

3\. User logs in → gets JWT token

4\. User browses Products page

5\. User clicks Add to Cart

6\. User proceeds to Checkout

7\. Order is placed and saved to MongoDB



\---



\## 6. MVC PATTERN



Model (models/):

\- User.js - User schema

\- Product.js - Product schema



View (client/src/pages/):

\- Home.js, Login.js, Register.js, Products.js



Controller (controllers/):

\- authController.js - handles login/register

\- productController.js - handles product operations



\---



\## Steps For Execution



1\. Clone the repository:

&#x20;  git clone https://github.com/mehermadhuri/shopez.git



2\. Setup Server:

&#x20;  cd shopez/server

&#x20;  npm install

&#x20;  Create .env file with:

&#x20;  PORT=5000

&#x20;  MONGO\_URI=your\_mongodb\_uri

&#x20;  JWT\_SECRET=shopez\_secret\_key\_2024

&#x20;  node server.js



3\. Setup Client:

&#x20;  cd shopez/client

&#x20;  npm install

&#x20;  npm start



4\. Open browser:

&#x20;  Frontend: http://localhost:3000

&#x20;  Backend:  http://localhost:5000



\---



\## GitHub Repository

https://github.com/mehermadhuri/shopez

