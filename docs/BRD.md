# Business Requirements 

---

## 1. Project Overview

Arogya is a full-stack healthcare appointment management system that allows patients to book appointments online, communicate with the clinic, and manage their profile. The platform includes an admin dashboard to oversee doctors, appointments, and messages.  
The system consists of a **Node.js + Express backend** and a **React-based frontend**, with separate interfaces for users and admin.

---

## 2. Business Problem

Patients currently face difficulty in:

- Booking appointments without calling or physically visiting.
- Tracking appointment status and doctor availability.
- Communicating health-related concerns digitally.

Admins struggle with:

- Managing doctor records manually.
- Handling appointment requests efficiently.
- Responding to patient messages across multiple channels.

---

## 3. Objectives

The system aims to:

- Enable patients to schedule and manage appointments online.
- Provide a digital communication channel between user and clinic.
- Allow admins to manage doctors, appointments, and messages centrally.
- Improve operational efficiency and reduce manual workload.
- Maintain secure authentication for both users and administrators.

---

## 4. High-Level Requirements

### **User Features**
- User can register
- User can login
- User can update profile
- User can book an appointment
- User can view appointment status/history
- User can send messages to clinic/admin

### **Admin Features**
- Admin can login
- Admin can manage doctor records (add/edit/delete)
- Admin can view and approve/reject appointments
- Admin can manage users
- Admin can view and respond to messages
- Admin can access dashboard analytics

### **System Requirements**
- Secure authentication and authorization
- Backend API handling (appointments, messages, users)
- Database connection for persistent storage
- Real-time or status-based update handling
- Separate portals for admin & user

---

## 5. Scope

### **In-Scope**
- Web-based patient portal
- Admin dashboard for clinic management
- Appointment scheduling and management
- User and admin authentication
- Messaging module between user and clinic
- Doctor management
- Database integration

### **Out-of-Scope**
- Mobile app version
- Online payment processing
- Prescription generation
- Video consultation or telemedicine
- Third-party hospital system integration (EMR/EHR)

---

## 6. Stakeholders

- **End User / Patient** – books appointments and communicates with clinic
- **Admin / Clinic Staff** – manages doctors, appointments, and messages
- **Doctor** – receives appointment requests (indirect stakeholder)
- **Developer Team** – builds and maintains the system
- **Business Analyst** – defines requirements and ensures alignment
- **Project Manager** – oversees delivery and timelines
