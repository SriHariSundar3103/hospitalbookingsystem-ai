# 🏥 AI Hospital Appointment System

<p align="center">

![React](https://img.shields.io/badge/Frontend-React-61DAFB?style=for-the-badge\&logo=react)
![Vite](https://img.shields.io/badge/Vite-646CFF?style=for-the-badge\&logo=vite)
![n8n](https://img.shields.io/badge/Automation-n8n-FF6D5A?style=for-the-badge\&logo=n8n)
![PostgreSQL](https://img.shields.io/badge/Database-PostgreSQL-4169E1?style=for-the-badge\&logo=postgresql)
![Gemini](https://img.shields.io/badge/LLM-Google_Gemini-4285F4?style=for-the-badge\&logo=google)
![Neon](https://img.shields.io/badge/Database-Neon-00E699?style=for-the-badge)
![JavaScript](https://img.shields.io/badge/JavaScript-ES6-F7DF1E?style=for-the-badge\&logo=javascript)

</p>

---

# 📌 Overview

The **AI Hospital Appointment System** is an intelligent appointment booking platform that automates the complete healthcare scheduling workflow using **Agentic AI, n8n automation, PostgreSQL, and a modern React frontend**.

Instead of manually managing hospital appointments, the AI understands natural language requests, identifies the appropriate medical department and doctor, checks doctor availability, validates existing patients, books appointments, updates doctor schedules, and automatically sends personalized confirmation or alternative-slot emails.

This project demonstrates how **Agentic AI and intelligent workflow automation can solve real-world healthcare scheduling challenges**.

---

# ✨ Features

### 🤖 AI-Powered Appointment Booking

* Understands natural language appointment requests
* Extracts structured patient information using Google Gemini
* Automatically identifies the appropriate department
* Selects the suitable doctor
* Checks doctor availability
* Suggests alternative appointment slots when unavailable

---

### 👤 Patient Management

* Detects whether a patient already exists
* Automatically creates new patient records
* Reuses existing patient information
* Reduces duplicate patient records

---

### 📅 Smart Appointment Scheduling

* Books appointments automatically
* Prevents double booking
* Updates doctor schedules
* Marks occupied appointment slots as unavailable
* Handles unavailable appointment requests intelligently

---

### 📧 Intelligent Email Notifications

Automatically sends:

#### ✅ Appointment Confirmation Email

Includes:

* Doctor Name
* Department
* Appointment Date
* Appointment Time
* Hospital Instructions
* Things to Bring
* Arrival Guidelines

#### ⚠️ Slot Unavailable Email

If the requested appointment slot is unavailable, the system automatically sends:

* Available Time Slots
* Available Dates
* Alternative Appointment Options
* Rebooking Form Link

---

### 💾 Database Automation

The AI workflow automatically manages and updates:

* Patients
* Doctors
* Doctor Schedule
* Appointments

No manual database intervention is required during the appointment booking workflow.

---

# 🛠 Tech Stack

## Frontend

* React
* Vite
* Tailwind CSS
* JavaScript ES6

## Backend Automation

* n8n

## Artificial Intelligence

* Google Gemini
* AI Agent
* Structured Output Parser

## Database

* PostgreSQL
* Neon Database

## Email Automation

* Gmail Node using n8n

## Deployment

* Vercel
* n8n Cloud

---

# 🧠 AI Workflow

```text
Patient fills Appointment Form
            │
            ▼
      AI Agent (Gemini)
            │
            ▼
 Extract Patient Information
            │
            ▼
 Find Doctor by Department
            │
            ▼
 Check Doctor Availability
            │
      ┌─────┴──────┐
      │            │
 Available      Not Available
      │            │
      ▼            ▼
Check Patient   Find Available Slots
      │            │
      ▼            ▼
Existing?     Send Alternative Email
      │
 ┌────┴────┐
 │         │
Yes       No
 │         │
 ▼         ▼
Book     Create Patient
 │
 ▼
Update Doctor Schedule
 │
 ▼
Send Confirmation Email
```

---

# 🗂 Database Schema

### Patients

* `patient_id`
* `patient_name`
* `email`
* `phone`
* `age`
* `gender`

---

### Doctors

* `doctor_id`
* `doctor_name`
* `department`
* `specialization`
* `available_days`
* `start_time`
* `end_time`

---

### Doctor Schedule

* `schedule_id`
* `doctor_id`
* `available_date`
* `appointment_time`
* `is_available`

---

### Appointments

* `appointment_id`
* `patient_id`
* `doctor_id`
* `appointment_date`
* `appointment_time`
* `symptoms`

---

# 📸 Screenshots

## 🏠 Home Page

![Home Page](images/home.png)

---

## 📅 Appointment Booking

![Appointment Booking](images/booking-form.png)

---

## 🤖 AI Automation Workflow

![AI Workflow](images/n8n-workflow.png)

---

## 📧 Appointment Confirmation Email

![Confirmation Email](images/confirmation-email.png)

---

## ⚠️ Slot Unavailable Email

![Slot Unavailable Email](images/slot-unavailable-email.png)

---

## 💾 PostgreSQL Database

![Database](images/database.png)

---

# 🚀 Appointment Workflow

1. Patient fills the appointment booking form.
2. AI extracts patient and appointment information.
3. The medical department is automatically identified.
4. The appropriate doctor is selected.
5. Doctor availability is checked.
6. Existing patient records are verified.
7. A new patient record is created if required.
8. The appointment is booked.
9. The doctor's schedule is updated.
10. A personalized confirmation email is sent.

### If the requested slot is unavailable:

* Alternative appointment slots are identified.
* Available dates and times are retrieved.
* An alternative-slot email is automatically sent.
* The patient can submit a new appointment request.

---

# 📂 Project Structure

```text
hospitalbookingsystem-ai
│
├── public
├── src
│   ├── assets
│   ├── components
│   ├── pages
│   ├── services
│   ├── utils
│   └── App.jsx
│
├── n8n
│   └── Hospital_Workflow.json
│
├── README.md
└── package.json
```

---

# ⚙️ Installation

### Clone the Repository

```bash
git clone https://github.com/SriHariSundar3103/hospitalbookingsystem-ai.git
```

### Move into the Project Directory

```bash
cd hospitalbookingsystem-ai
```

### Install Dependencies

```bash
npm install
```

### Run the Development Server

```bash
npm run dev
```

---

# 🌐 Live Demo

### 🚀 AI Hospital Appointment System

https://hospitalbookingsystem-ai.vercel.app/

---

# 🔮 Future Improvements

* WhatsApp Appointment Notifications
* Appointment Cancellation
* Appointment Rescheduling
* Doctor Dashboard
* Admin Dashboard
* Patient Authentication
* Patient Medical History
* PDF Prescription Generation
* Online Payment Gateway
* Google Calendar Integration
* SMS Notifications
* AI Medical Assistant
* Multi-Hospital Support
* Doctor Analytics Dashboard

---

# 👨‍💻 Author

## Sri Hari Sundar R.

**B.E. Computer Science and Engineering**

### 📧 Email

[sri352006@gmail.com](mailto:sri352006@gmail.com)

### 💼 LinkedIn

[www.linkedin.com/in/srihari-sundar](http://www.linkedin.com/in/srihari-sundar)

### 🐙 GitHub

https://github.com/SriHariSundar3103

### 📂 Project Repository

https://github.com/SriHariSundar3103/hospitalbookingsystem-ai/tree/main

### 🌐 Live Project

https://hospitalbookingsystem-ai.vercel.app/

---

# ⭐ Support

If you found this project useful, consider giving it a ⭐ on GitHub.

Your support helps others discover the project and motivates future improvements.

---

<p align="center">

### 🚀 Built with Agentic AI, n8n Automation, React, Gemini & PostgreSQL

**Developed by Sri Hari Sundar R.**

</p>

