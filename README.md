StageLink

StageLink is a secure multi-school internship tracking, application, and document management platform. It is developed as an end-of-year project by a group of 5 EMSI Tanger students for the academic year 2025/2026. Its goal is to connect students, companies, schools, and platform administrators in one secure and organized system.

The platform helps schools supervise student internship activity, verify student identities, manage internship documents securely, and allow verified companies to publish internship opportunities in a controlled environment.

Project Overview

Internship management is often fragmented:

students search and apply in unstructured ways
companies receive many files without verification
schools have limited visibility on student internship progress
documents are often shared without proper control
there is no clear tracking of user actions

StageLink solves this by offering a centralized platform where:

schools can join the platform after approval
students register under their own school and get verified by that school
companies create accounts and get verified before publishing offers
school admins track student internship activity, documents, and progress
super admins supervise schools, companies, and global system activity

The project is strongly aligned with these main themes:

secure authentication
secure document management
user action logging
Main Objective

The objective of StageLink is to build a secure and scalable platform that allows multiple schools to supervise internship activities of their students while ensuring controlled access, document protection, and full action traceability.

Main Users
Student

A student can:

create an account
choose their school during registration
upload a student card for verification
wait for approval from their school
complete a personal profile
upload internship-related documents
browse internship offers
apply for internships
track application progress
Company

A company can:

create an account
submit company information for verification
wait for approval before accessing full features
publish internship offers
review student applications
access authorized documents
update application status
School Admin

A school administrator can:

manage their school space
review and approve student accounts
verify uploaded student cards
monitor student internship activity
supervise student documents
track internship progress
consult school dashboard and statistics
Super Admin

A super admin can:

approve or reject schools
approve or reject companies
monitor all platform activity
manage global users and roles
supervise security and logs
access global dashboard statistics
Core Workflows
1. School Approval Workflow

StageLink is not limited to one school.

A school can request access to the platform:

the school submits its registration request
the request is reviewed by the super admin
the school is approved or rejected
once approved, the school can manage its own students through its admins

This ensures that only verified institutions can join the platform.

2. Student Verification by School

When a student signs up:

the student creates an account
the student selects their school
the student uploads a scanned student card
the account is marked as pending
the school admin of that school reviews the request
the account is approved or rejected
only approved students can fully use the platform

This process ensures that each student is validated by their own institution.

3. Company Verification

To reduce fake or untrusted company accounts:

the company creates an account
the company submits its information
the account remains pending
the super admin verifies the company
only approved companies can publish internship offers

This improves platform trust and quality.

Main Features
secure registration and login
multi-level role management
school approval workflow
student verification by school
company verification
secure document upload and access control
internship offer management
internship application tracking
dashboard for supervision and monitoring
user action logging and audit trail
Functional Modules
1. Authentication and Authorization
registration
login
password protection
role-based access control
protected routes
account status management
2. Multi-Level Roles

The system includes multiple roles:

Super Admin
School Admin
Company
Student

Each role has different permissions and access levels.

3. School Management
school registration request
school approval or rejection
school-specific administration
school-specific student tracking
4. Student Management
registration under a selected school
upload student card
verification request handling
school-based validation
student profile management
5. Company Management
company registration
company verification workflow
offer publication
applicant management
6. Secure Document Management
upload CVs and internship documents
store file references securely
controlled file access by role
authorized document viewing and download
restricted access for unauthorized users
7. Internship Management
create internship offers
browse internship offers
apply to internship offers
manage application status
track internship progress
8. Dashboard and Monitoring

The platform includes dashboards for supervision.

Examples of dashboard information:

total schools
total verified schools
total students
verified students
pending student verifications
total companies
verified companies
total offers
total applications
internship status statistics
9. Logging System

The platform records important actions such as:

school registration
school approval
company registration
company approval
student registration
student card upload
student approval or rejection
login attempts
profile updates
document upload
document access
internship application submission
application status updates
admin moderation actions

This module improves security, accountability, and traceability.

Why This Project Is Strong

StageLink is more than a basic internship site.

It becomes a secure multi-school supervision platform with:

institution onboarding
student identity verification
company verification
secure document control
multi-role access management
administrative dashboards
logs and audit history

This makes the project:

more realistic
more scalable
more professional
more original
strongly aligned with backend and database design
Technologies Used
Frontend
React
Tailwind CSS
React Router
Axios
Backend
Laravel
Database
MySQL
Tools
Git & GitHub
VS Code
Postman
Figma (optional)
Suggested Database Entities
schools
id
name
email
city
address
status
verified_at
created_at
users
id
school_id
name
email
password
role
status
created_at
students
id
user_id
school_id
student_number
department
academic_year
student_card_path
validation_status
validated_by
validated_at
companies
id
user_id
company_name
sector
description
website
city
verification_status
verified_at
offers
id
company_id
title
description
location
duration
deadline
status
applications
id
student_id
offer_id
status
applied_at
documents
id
student_id
type
file_path
uploaded_at
logs
id
user_id
action
target_type
target_id
description
created_at
Example Use Cases
a school requests access to the platform
the super admin approves the school
a student registers and selects their school
the student uploads a student card
the school admin validates the student
a company registers and gets approved
the company publishes an internship offer
a verified student applies for the internship
the school tracks the student’s internship progress
the system records all important actions in logs
Project Structure
StageLink/
│
├── frontend/        # React application
├── backend/         # Laravel API
├── database/        # Migrations and seeders
├── docs/            # UML diagrams, reports, notes
└── README.md

Future Work

In future versions, StageLink can be improved by adding a small intelligent module to support students, schools, and companies. This AI part is not a core requirement of the first version. The first version should stay focused on security, stability, verification workflows, document management, internship tracking, dashboards, and action logging.

Possible future AI-based improvements include:

internship recommendation system
suggest internship offers to students based on their profile, skills, academic background, and application history
match score calculation
compare a student profile with internship requirements and generate a compatibility score
skill gap detection
show missing skills that a student should improve to better match a specific internship offer
basic CV analysis
extract useful keywords, skills, or technologies from uploaded CVs to improve recommendations
smart dashboard insights
help admins identify trends such as the most requested skills, most active companies, or common application patterns. This is a natural extension of the intelligent features described in the earlier project context.
Conclusion

StageLink is not just a simple internship website. It is a secure multi-school platform designed to improve internship supervision, student verification, company trust, secure document handling, and administrative monitoring in one system. Its architecture also allows future improvements without rebuilding the whole platform.
