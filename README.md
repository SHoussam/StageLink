# StageLink

**StageLink** is a secure web platform for **internship tracking, application management, and document supervision**.  
It is developed as an **end-of-year project (PFA)** by **Group 5** at **EMSI Tanger** for the academic year **2025/2026**.

The platform connects **students, companies, and school administrators** in one system.

Its main purpose is to make internship management more secure, more organized, and easier to supervise inside the school.

---

## Project Idea

In many schools, internship applications are often managed in a scattered way.  
Students search for opportunities by themselves, companies receive many files without structure, and schools have limited visibility on student internship activity.

**StageLink** solves this problem by providing a centralized platform where:

- students can register, upload their documents, and apply for internships
- companies can publish offers and review applicants
- schools can track student internship activity, validate student accounts, supervise documents, and monitor the overall process

The project is designed around the themes assigned to **Group 5**:

- **secure authentication**
- **secure document management**
- **user action logging**

---

## Main Objective

The goal of StageLink is to build a secure and organized platform that allows schools to monitor internship activity while helping students and companies manage the internship process more efficiently.

---

## Main Users

### Student
A student can:

- create an account
- submit registration information
- upload a student card for validation
- complete a personal profile
- upload internship-related documents
- browse internship offers
- apply for internships
- track application status

### Company
A company can:

- create an account
- publish internship offers
- review student applications
- access authorized candidate documents
- update application status

### School Admin
A school administrator can:

- validate student accounts
- verify uploaded student cards
- monitor student internship activity
- supervise documents
- track applications and internship progress
- manage platform users
- consult logs and statistics

---

## Student Validation Process

One of the important ideas in this project is **student identity validation**.

When a student signs up:

1. the student creates an account
2. the student uploads a scanned image or file of their **student card**
3. the account is marked as **pending**
4. a **school administrator** reviews the information
5. the admin approves or rejects the account
6. only approved students can fully use the platform and apply for internships

This makes the system more secure and ensures that only real students from the school can access the platform.

---

## Main Features

- Secure registration and login
- Role-based access control
- Student account validation by school admin
- Student card upload during registration
- Secure document upload and storage
- Controlled access to files based on user role
- Internship offer management
- Internship application management
- Activity tracking with logs
- Admin dashboard for supervision and monitoring

---

## Functional Modules

### 1. Authentication and Authorization
- registration
- login
- password protection
- role-based access control
- protected routes
- account status management (`pending`, `approved`, `rejected`)

### 2. Student Validation
- upload student card
- save verification request
- admin review of student information
- approve or reject student account
- store validation history

### 3. Secure Document Management
- upload CVs and internship documents
- store files securely
- control access based on roles
- allow only authorized users to view or download files
- restrict unauthorized access

### 4. Internship Offer Management
- companies create internship offers
- companies edit or delete offers
- students browse offers
- students apply to offers
- companies manage applicant status

### 5. School Supervision
- track student internship activity
- view applications by student
- verify required documents
- monitor progress of internships
- access platform statistics

### 6. Logging System
The platform records important user actions such as:

- registration
- login
- student card upload
- student account approval or rejection
- document upload
- document access
- internship application submission
- application status updates
- profile modifications
- admin moderation actions

This module improves traceability, supervision, and security.

---

## Why This Project Is Interesting

StageLink is more than a simple internship website.

It adds a strong academic and administrative value because the school is directly involved in the process.

The platform allows the school to:

- verify student identity
- track internship applications
- supervise internship documents
- monitor progress and activity
- maintain a clear history of actions through logs

This makes the project more realistic, more secure, and more professional.

---

## Technologies Used

### Frontend
- React
- Tailwind CSS
- React Router
- Axios

### Backend
- Laravel

### Database
- MySQL

### Tools
- Git & GitHub
- VS Code
- Postman
- Figma (optional)

---

## System Roles

The platform is based on **three main roles**:

- **Student**
- **Company**
- **School Admin**

Each role has specific permissions and access levels.

---

## Suggested Database Entities

### `users`
- id
- name
- email
- password
- role
- status
- created_at

### `students`
- id
- user_id
- student_number
- department
- academic_year
- student_card_path
- validation_status
- validated_by
- validated_at

### `companies`
- id
- user_id
- company_name
- sector
- description
- website
- city

### `offers`
- id
- company_id
- title
- description
- location
- duration
- deadline
- status

### `applications`
- id
- student_id
- offer_id
- status
- applied_at

### `documents`
- id
- student_id
- type
- file_path
- uploaded_at

### `logs`
- id
- user_id
- action
- target_type
- target_id
- description
- created_at

---

## Example Use Cases

- A student registers and uploads a student card
- The school admin validates the student account
- A student uploads a CV
- A company publishes a new internship offer
- A student applies to the offer
- A company reviews the application
- The school checks the student’s internship activity
- The system records all major actions in logs

---

## Project Structure

```bash
StageLink/
│
├── frontend/        # React application
├── backend/         # Laravel API
├── database/        # Migrations and seeders
├── docs/            # UML diagrams, reports, notes
└── README.md
