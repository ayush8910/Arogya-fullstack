# Functional Requirements

---

## 1. System Features

- User Registration
- User Login & Authentication
- User Profile Management
- Appointment Booking
- Appointment Status & History View
- User Messaging to Clinic/Admin
- Admin Login
- Admin Dashboard
- Doctor Management (Add/Edit/Delete)
- Appointment Management (Approve/Reject/View)
- User Management (View/Delete)
- Message Management (Respond to inquiries)
- Database Connectivity & Persistence
- Secure Authorization (User vs Admin roles)

---

## 2. Functional Requirements (per feature)

### **User Registration**
- Validate required fields (name, email, password)
- Validate unique email
- Validate email format
- Save user data to database
- Encrypt password before saving

### **User Login**
- Validate email and password
- Authenticate against stored credentials
- Generate secure token/session
- Redirect user to dashboard

### **User Profile Management**
- Fetch user profile data
- Allow update of fields (name, contact, etc.)
- Validate input formats
- Save updated data

### **Appointment Booking**
- Display available doctors
- Select date and time
- Validate time slot availability
- Save appointment request
- Notify admin of new request

### **Appointment Status & History**
- Fetch user’s upcoming and past appointments
- Display approval/rejection status
- Allow cancellation (if supported)

### **User Messaging**
- Validate message content
- Save message in backend
- Display previous messages
- Notify admin of new message

### **Admin Login**
- Validate admin credentials
- Provide access only to admin-specific routes
- Redirect to admin dashboard

### **Admin Dashboard**
- Display total counts (users, doctors, appointments, messages)
- View summary charts or statistics (if available)

### **Doctor Management**
- Add new doctor with details
- Edit existing doctor info
- Delete doctor record
- Validate unique doctor data (email/name)

### **Appointment Management**
- View all appointment requests
- Approve or reject appointment
- Update appointment status
- Notify user of status change

### **User Management**
- View registered users
- Delete/remove users (if required)
- Fetch user-related data

### **Message Management**
- View messages from users
- Respond to messages
- Mark message as addressed

---

## 3. User Flow Diagrams

*(Placeholder – PNGs can be added later)*

Example:

- `user_flow_registration.png`
- `appointment_booking_flow.png`
- `admin_dashboard_flow.png`

---

## 4. Field Validations

### **User Fields**
- Name: required, alphabets only
- Email: must be valid format & unique
- Password: minimum 8 characters, encrypted
- Phone (optional): numeric, 10 digits

### **Appointment Fields**
- Date: must be a valid future date
- Time: must match available slots
- Doctor ID: must exist in system

### **Doctor Fields**
- Name: required
- Specialization: required
- Email: valid & unique

### **Message Fields**
- Content: cannot be empty
- Max length: 500 characters

---

## 5. API References (optional)

### **Authentication**
- `POST /register` – create new user
- `POST /login` – authenticate user
- `POST /admin/login` – admin authentication

### **Appointments**
- `POST /appointments` – book appointment
- `GET /appointments/user/:id` – get user's appointments
- `PATCH /appointments/:id/status` – admin update status

### **Doctors**
- `POST /doctors` – add doctor
- `GET /doctors` – list doctors
- `DELETE /doctors/:id` – remove doctor

### **Messages**
- `POST /messages` – send message
- `GET /messages` – admin view messages
