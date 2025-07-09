# 🏥 QuickMed Backend – Powering Healthcare Appointments & Prescriptions 🚀

QuickMed Backend is the **secure and scalable** API powering **QuickMed**, a modern healthcare appointment and prescription management system.  
It handles **user authentication, doctor profiles, appointment bookings, prescriptions, and payments**, ensuring a seamless healthcare experience.

🔹 **Built with Node.js, Express, and MongoDB**  
🔹 **Secure JWT authentication & role-based access**  
🔹 **RESTful API for smooth frontend communication**  
🔹 **Integrated Razorpay payment gateway**

---

## 🌐 API Base URL

🔗 **[https://your-backend-api.com](https://your-backend-api.com)**

📢 **Note:** This repository contains only the **backend** code.  
For the frontend, visit: **[QuickMed Frontend](https://github.com/itxnargis/QuickMed)**.

---

## 📖 Table of Contents

- [✨ Features](#-features)
- [🛠 Technologies Used](#-technologies-used)
- [⚙️ API Endpoints](#-api-endpoints)
- [🚀 Installation](#-installation)
- [🕹 Usage](#-usage)
- [🤝 Contributing](#-contributing)
- [📄 License](#-license)

---

## ✨ Features

✅ **User Authentication** – Secure JWT-based login & registration  
✅ **Role-Based Access** – Patients, Doctors, and Admins  
✅ **Doctor Management** – Add, update, and fetch doctor details  
✅ **Appointment Scheduling** – Book, reschedule, and cancel appointments  
✅ **Prescription Management** – Issue & store prescriptions digitally  
✅ **Secure Payments** – Integrated Razorpay for easy transactions  
✅ **API Documentation** – Comprehensive Swagger docs for developers

---

## 🛠 Technologies Used

- **Backend:** Node.js, Express.js
- **Database:** MongoDB (Mongoose ORM)
- **Authentication:** JWT (JSON Web Token)
- **Payments:** Razorpay API
- **Validation:** Joi for input validation
- **Environment Management:** dotenv
- **Logging:** Morgan

---

## ⚙️ API Endpoints

### **🔑 Authentication**

- `POST /api/auth/register` – Register a new user
- `POST /api/auth/login` – Login & receive a JWT token

### **👨‍⚕️ Doctor Management**

- `GET /api/doctors` – Fetch all doctors
- `GET /api/doctors/:id` – Get doctor details
- `POST /api/doctors` – Add a doctor (Admin)
- `PUT /api/doctors/:id` – Update doctor info (Admin)
- `DELETE /api/doctors/:id` – Remove a doctor (Admin)

### **📅 Appointments**

- `POST /api/appointments` – Book an appointment
- `GET /api/appointments/:id` – Get appointment details
- `PUT /api/appointments/:id` – Reschedule/cancel an appointment

### **💊 Prescriptions**

- `GET /api/prescriptions` – View patient prescriptions
- `POST /api/prescriptions` – Issue a prescription (Doctor)

### **💳 Payments**

- `POST /api/payments` – Process payments via Razorpay
- `GET /api/payments/:id` – Get payment status

📌 **More endpoints available in API documentation.**

---

## 🚀 Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/yourusername/QuickMed-backend.git
   cd QuickMed-backend

   ```
2. **Install Dependencies**

   ```bash
   npm install

   ```

3. **Configure environment**

   ```bash
   PORT=5000
   MONGO_URI=your_mongodb_connection_string
   JWT_SECRET=your_jwt_secret
   RAZORPAY_KEY=your_razorpay_key
   RAZORPAY_SECRET=your_razorpay_secret

   ```

4. **Start the server**

   ```bash
   npm start

   ```

5. **Your API will be live at http://localhost:5000.**

## 🕹 Usage

1️⃣ **Register & Login** – Authenticate users securely

- Patients and doctors can create accounts and log in using JWT-based authentication.
- Secure password hashing ensures data protection.

2️⃣ **Manage Doctors** – Fetch & update doctor profiles

- Patients can browse a list of verified doctors based on specialty and availability.
- Admins can add, update, or remove doctor profiles.

3️⃣ **Book Appointments** – Schedule & track medical visits

- Patients can select a doctor and book an available appointment slot.
- Appointments can be rescheduled or canceled if needed.

4️⃣ **Handle Prescriptions** – Issue & view patient prescriptions

- Doctors can issue digital prescriptions after consultations.
- Patients can access their prescription history anytime.

5️⃣ **Process Payments** – Secure transactions via Razorpay

- Patients can pay for consultations using Razorpay's secure payment gateway.
- Payment status and transaction details are stored for reference.

## 🤝 Contributing

Contributions are welcome! Please follow these steps:

1. Fork the project.
2.
3. Create your feature branch:
   ```bash
   git checkout -b feature/new-feature

   ```
4. Commit your changes:
   ```bash
   git commit -m "Add new feature"

   ```
5. Push to the branch:
   ```bash
   git push origin feature/new-feature

   ```
6. Open a Pull Request.
