# stayfinder – Airbnb Clone Full Stack App

StayFinder is a full-stack web application that allows users to register, browse property listings, and make bookings for short- or long-term stays. Hosts can post listings, and users can search, view, and book available accommodations.

---

## 🌐 Tech Stack

### Frontend
- React.js (not included in this repo – to be built in /frontend folder)

### Backend
- Node.js
- Express.js
- MongoDB + Mongoose
- JWT for authentication
- bcryptjs for password hashing
- dotenv for environment variables

---

## 📁 Folder Structure (Backend)
```
stayfinder/
└── backend/
    ├── server.js
    ├── .env
    ├── models/
    │   ├── User.js
    │   ├── Listing.js
    │   └── Booking.js
    ├── routes/
    │   ├── auth.js
    │   ├── listings.js
    │   └── bookings.js
```

---

## 🔐 Environment Variables (.env)
```
PORT=5000
MONGO_URI=mongodb://localhost:27017/stayfinder
JWT_SECRET=yourSecretKey
```

> Make sure to add `.env` to `.gitignore`

---

## 🚀 Getting Started (Backend)

```bash
# Navigate to backend folder
cd backend

# Install dependencies
npm install

# Start the server
npm run dev
```

---

## ✅ API Endpoints

### Auth
- `POST /api/auth/register` – User registration
- `POST /api/auth/login` – User login (returns JWT token)

### Listings
- `GET /api/listings` – Get all listings
- `GET /api/listings/:id` – Get single listing
- `POST /api/listings` – Create listing (requires host)

### Bookings
- `POST /api/bookings` – Book a listing

---

## 🧪 Seed Sample Listing
Use Postman or MongoDB Compass to add:
```json
{
  "title": "Beach House in Goa",
  "description": "A relaxing 2BHK with ocean view.",
  "location": "Goa",
  "price": 3500,
  "image": "https://source.unsplash.com/800x600/?beachhouse",
  "hostId": "<insert_host_user_id>"
}
```

---

## 🔐 Security Notes
- Passwords hashed with bcrypt
- JWT tokens used for login auth
- CORS enabled

---

## ✨ Features To Add Later (Optional)
- Search filters by location, price, date
- Booking calendar & date availability check
- Host dashboard
- Stripe integration for payments
- Google Maps integration

---

## 🧠 Unique Features (Suggestions)
1. Group trip planning (vote on listings)
2. Smart recommendations based on booking history

---

## 🧑‍💻 Author
This project was completed as part of an internship by [Your Name] for StayFinder Full Stack Internship Program 2025.

---

Let me know if you want help with the frontend scaffold, booking calendar, or Stripe integration!
