📘 Booking System API

A simple and clean back-end REST API for managing hotel room bookings (or general appointments).
This project is built for the ALX Back-End Professional Foundations – Final Project.

🚀 Features

User Registration & Login (JWT Authentication)

Hotel Room Management (CRUD)

Booking Management (Create, View, Cancel)

Prevent double booking with server-side validation

Simple, clean REST API following best practices

Uses a relational database (MySQL / PostgreSQL)

Seed data for quick testing

🏗️ Tech Stack
Layer	Technology
Backend Framework	Node.js + Express
Database	MySQL (or PostgreSQL)
ORM	Prisma ORM
Authentication	JWT
Environment Config	dotenv
API Testing	Thunder Client / Postman
📁 Project Structure
project/
│── src/
│   ├── config/
│   ├── controllers/
│   ├── middleware/
│   ├── routes/
│   ├── prisma/
│   ├── utils/
│   └── app.js
│
│── prisma/
│   └── schema.prisma
│
├── .env
├── package.json
└── README.md

🔧 Installation & Setup
1️⃣ Clone the repo
git clone https://github.com/<your-username>/booking-system.git
cd booking-system

2️⃣ Install dependencies
npm install

3️⃣ Configure .env
DATABASE_URL="mysql://root:password@localhost:3306/booking_db"
JWT_SECRET="supersecretkey"
PORT=3000

4️⃣ Push database schema
npx prisma migrate dev --name init

5️⃣ Start the server
npm start

🧪 API Endpoints
👤 Auth
Method	Endpoint	Description
POST	/api/auth/register	Register new user
POST	/api/auth/login	Login & get JWT token
🏨 Rooms
Method	Endpoint	Description
GET	/api/rooms	List all rooms
POST	/api/rooms	Create a room (Admin)
GET	/api/rooms/:id	Get room details
PUT	/api/rooms/:id	Update room
DELETE	/api/rooms/:id	Delete room
📅 Bookings
Method	Endpoint	Description
POST	/api/bookings	Create a new booking
GET	/api/bookings	View user bookings
DELETE	/api/bookings/:id	Cancel a booking
⚠️ Double Booking Prevention

The system prevents booking the same room in overlapping dates using server-side validation before creating a booking.

📝 Example Booking Request
POST /api/bookings
Content-Type: application/json

{
  "roomId": 1,
  "startDate": "2025-01-10",
  "endDate": "2025-01-15"
}

🎯 Project Goals (For ALX Review)

✔ Build a functional REST API
✔ Database design & modeling
✔ Implement authentication & validation
✔ Clean architecture & documentation
✔ Realistic real-world back-end project

👨‍💻 Author

Mostafa Khamis
ALX Back-End Professional Foundations Student