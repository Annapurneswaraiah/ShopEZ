# 🛍️ ShopEZ – One-Stop Shop for Online Purchases

ShopEZ is a full-stack e-commerce web application developed as part of the SmartInternz Internship Program.  
Built using the **MERN stack** (MongoDB, Express.js, React.js, Node.js), it provides users with a seamless shopping experience and allows admins to manage products, users, and orders efficiently.


## 🚀 Features

### 👤 User Features
- User Registration & Login
- Browse products with filters
- Add to cart
- Secure checkout
- Order confirmation
- Order history

### 🛠 Admin Features
- Admin dashboard
- Add/Edit/Delete products
- Manage orders
- View users
- Monitor activity

### 🎯 Core Functionalities
- Responsive UI
- JWT authentication
- REST API integration
- MongoDB database
- Modular architecture


## 🧰 Tech Stack

**Frontend:** React.js, JavaScript, CSS, Bootstrap  
**Backend:** Node.js, Express.js  
**Database:** MongoDB with Mongoose  
**Version Control:** Git & GitHub  
**Development Tools:** VS Code  


## 📁 Project Structure

SHOPEZ/
client/     → Frontend (React)
server/     → Backend (Node + Express)
README.md   → Project documentation


## ⚙️ Installation & Setup

### 1️⃣ Clone Repository

git clone https://github.com/suprajaK-dev/ShopEZ.git

### 2️⃣ Install Dependencies

**Frontend**

cd client
npm install

**Backend**

cd ../server
npm install


### 3️⃣ Environment Variables

Create a `.env` file inside the **server folder** and add:

PORT=5000
MONGO_URI=your_mongodb_connection_string
JWT_SECRET=your_secret_key


## ▶️ Running the Application

**Start Backend**

cd server
npm start

**Start Frontend**

cd client
npm start

App runs at:

http://localhost:3000


## 🔗 API Endpoints

### Auth

POST /api/register
POST /api/login
GET  /api/profile

### Products

GET    /api/products
GET    /api/products/:id
POST   /api/products
PUT    /api/products/:id
DELETE /api/products/:id

### Cart

POST   /api/cart/add
GET    /api/cart/:userId
DELETE /api/cart/remove/:id

### Orders

POST /api/orders
GET  /api/orders/:userId
GET  /api/orders/admin


## 🔐 Authentication

Authentication is handled using JSON Web Tokens (JWT)

**Flow**
1. User logs in  
2. Server validates credentials  
3. Token generated  
4. Token stored client-side  
5. Token sent with protected requests  

**Security Measures**
- Password hashing
- Token expiration
- Protected routes


## 🧪 Testing

Testing methods used:
- Manual testing
- API testing using Postman
- Form validation tests
- Authentication tests


## 📊 Results

✔ User authentication works  
✔ Products load dynamically  
✔ Cart operations function correctly  
✔ Orders stored successfully  
✔ Admin dashboard manages data  


## ⚠ Known Issues
- Payment gateway not integrated
- Basic recommendation logic
- No real-time notifications


## 🔮 Future Enhancements
- Payment integration (Stripe/Razorpay)
- AI recommendations
- Wishlist feature
- Push notifications
- Mobile app version
- Multi-vendor support


## 🙏 Acknowledgements
- SmartInternz for providing this project as an internship assignment  
- Original concept inspiration from Josan George’s version
