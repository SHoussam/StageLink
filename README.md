# StageLink

### Smart Internship & Recruitment Platform for Students, Companies, and Admins

StageLink is a web-based platform designed to simplify the internship search and recruitment process.  
It helps **students** find opportunities that match their skills, allows **companies** to publish internship offers and manage applicants, and gives **admins** a way to supervise the whole platform.

The project also includes a **small AI module** that improves the experience by recommending internships, calculating match scores, and analyzing student skills from profiles or CVs.

---

## Table of Contents

- [Project Overview](#project-overview)
- [Problem Statement](#problem-statement)
- [Objectives](#objectives)
- [Main Users](#main-users)
- [Main Features](#main-features)
- [AI Features](#ai-features)
- [Tech Stack](#tech-stack)
- [System Architecture](#system-architecture)
- [Database Design](#database-design)
- [Platform Workflow](#platform-workflow)
- [Installation](#installation)
- [Project Structure](#project-structure)
- [Team Work Distribution](#team-work-distribution)
- [Future Improvements](#future-improvements)
- [Conclusion](#conclusion)

---

## Project Overview

Finding internships is often difficult for students because opportunities are scattered across many platforms, and companies also spend time sorting through many applications to find suitable candidates.

CareerConnect AI solves this problem by offering a centralized platform where:

- Students can create profiles, upload CVs, and apply for internships
- Companies can post internship offers and manage applications
- Admins can supervise users, offers, and platform activity
- An AI-based recommendation system can suggest the best internships for each student

This project was developed as an **end-of-year web project** by a group of 4 students.

---

## Problem Statement

Students often face several challenges when looking for internships:

- Difficulty finding relevant internship offers
- Lack of personalized recommendations
- Limited visibility of their profiles and skills
- No simple way to track applications

At the same time, companies face challenges such as:

- Receiving many irrelevant applications
- Difficulty identifying the best candidates
- Time-consuming recruitment processes

This project aims to create a smart solution that connects students and companies more efficiently.

---

## Objectives

The main objectives of this project are:

- Build a modern and responsive web platform for internship management
- Allow students to create profiles and apply for internships
- Allow companies to post and manage internship offers
- Implement role-based access for students, companies, and admins
- Integrate a small AI module for recommendations and match scoring
- Provide dashboards and statistics for better decision-making

---

## Main Users

### 1. Student
A student can:

- Create an account and log in
- Complete a personal profile
- Add skills and academic information
- Upload a CV
- Search and filter internship offers
- Apply for internships
- Save offers for later
- View recommended internships
- Track application status

### 2. Company
A company can:

- Create a recruiter/company account
- Complete a company profile
- Publish internship offers
- Edit or delete offers
- View applicants for each offer
- Filter and rank candidates
- Manage application status

### 3. Admin
An admin can:

- Manage all users
- Validate or remove internship offers
- Monitor platform activity
- Access statistics and analytics
- Supervise reports and moderation

---

## Main Features

### Authentication & Authorization
- User registration and login
- Secure authentication
- Role-based access control
- Profile editing

### Student Features
- Personal profile management
- Skills management
- CV upload
- Internship browsing
- Filters by city, domain, type, and skills
- Application history
- Saved offers
- Dashboard with recommendations and statistics

### Company Features
- Company profile management
- Add, edit, and delete internship offers
- View applicants for each offer
- Change application status:
  - Pending
  - Reviewed
  - Accepted
  - Rejected
- Dashboard with statistics

### Admin Features
- User management
- Internship offer moderation
- Platform monitoring
- Global statistics dashboard

---

## AI Features

One of the strongest parts of this project is the integration of a **small AI module**.

### 1. Internship Recommendation System
The system compares student skills with internship requirements and calculates a **match score**.

Example:
- Student skills: PHP, MySQL, Laravel, React
- Offer requirements: PHP, Laravel, MySQL
- Result: 85% match

### 2. CV / Skill Analysis
The platform can analyze a student profile or CV to:

- Extract important skills
- Detect missing skills
- Suggest better matching opportunities

### 3. Candidate Ranking
For companies, the system can help rank candidates based on:

- Skill compatibility
- Preferred location
- Study level
- Internship domain

### Example of Matching Formula
```text
Match Score =
( matched_skills / required_skills ) * 70
+ city_match * 10
+ domain_match * 10
+ level_match * 10
