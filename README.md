# StageLink
### Smart Internship, Employability & Recruitment Platform

StageLink is a web-based platform designed to connect **students**, **companies**, and **academic institutions** in one intelligent ecosystem.  
It helps students find internships, helps companies identify suitable candidates, and helps schools monitor internship placement and market trends.

Unlike a simple internship board, StageLink is designed as an **employability platform**: it not only allows students to apply for offers, but also helps them understand their strengths, detect missing skills, and improve their readiness for the job market.

---

## Table of Contents

- [Project Overview](#project-overview)
- [Problem Statement](#problem-statement)
- [Main Objectives](#main-objectives)
- [What Makes StageLink Different](#what-makes-stagelink-different)
- [Main Users](#main-users)
- [Core Features](#core-features)
- [AI & Smart Features](#ai--smart-features)
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

Finding internships is often difficult for students because opportunities are scattered across different websites, and many students do not know whether their profile really matches the market.  
At the same time, companies often receive many applications and need a better way to identify the most relevant candidates.

StageLink solves this problem by providing a centralized platform where:

- **Students** can create profiles, add skills, upload CVs, receive recommendations, and apply for internships
- **Companies** can publish offers, manage candidates, and review ranked applicants
- **Schools/Admins** can monitor internship placement, student progress, and market demand

The platform also includes a **small intelligent recommendation module** that calculates match scores, explains why an offer matches a student, and highlights missing skills.

---

## Problem Statement

Students face several challenges when searching for internships:

- Difficulty finding opportunities adapted to their profile
- Lack of guidance on which skills they need to improve
- No clear explanation of why a specific internship fits them
- No simple way to track applications and progress

Companies also face challenges such as:

- Receiving many irrelevant applications
- Difficulty identifying the best candidates quickly
- Lack of intelligent filtering and ranking tools

Schools and coordinators may also struggle to:

- Track student placement
- Understand market demand
- Follow internship activity across students and companies

StageLink is designed to address all of these problems in one platform.

---

## Main Objectives

The main objectives of this project are:

- Build a modern and responsive internship web platform
- Allow students to search and apply for internships
- Allow companies to publish offers and manage applicants
- Provide admins/schools with monitoring and analytics tools
- Implement role-based authentication and dashboards
- Add a small intelligent recommendation system
- Improve student employability through skill-gap guidance
- Create a scalable project that can evolve in future versions

---

## What Makes StageLink Different

StageLink is not just another internship listing website.

### 1. School-Connected Platform
StageLink includes an academic/admin perspective.  
In addition to students and companies, it can also help schools or coordinators:

- track student placements
- monitor active companies
- view internship statistics
- analyze the most demanded skills in the market

### 2. Explainable AI Matching
Instead of only showing a score, StageLink explains **why** an internship matches a student.

Example:
- Match Score: **82%**
- 3 out of 4 required skills matched
- City preference matched
- Profile level matched
- Missing skill: **Docker**

This makes the system more transparent and more useful.

### 3. Employability Growth Approach
StageLink is not only made to help students apply.  
It is also designed to help them **become internship-ready** by offering:

- profile completion indicators
- skill-gap detection
- personalized recommendations
- career-readiness support

---

## Main Users

### 1. Student
A student can:

- Create an account and log in
- Complete a personal profile
- Add skills and academic information
- Upload a CV
- Search and filter internship offers
- Save offers for later
- Apply for internships
- Track application status
- Receive recommended internships
- View missing skills for selected offers

### 2. Company
A company can:

- Create a recruiter/company account
- Complete a company profile
- Publish internship offers
- Edit or delete offers
- View applicants for each offer
- Review candidate match scores
- Rank or filter candidates
- Update application status

### 3. Admin / School Coordinator
An admin or coordinator can:

- Manage users and internship offers
- Monitor student placement
- View statistics and analytics
- Track active companies
- Analyze trends in required skills and internship demand

---

## Core Features

### Authentication & Authorization
- User registration and login
- Secure authentication
- Role-based access control
- Profile management

### Student Features
- Personal profile creation
- Skills management
- CV upload
- Internship browsing
- Search and filters
- Saved offers
- Application tracking
- Personalized dashboard

### Company Features
- Company profile management
- Add, edit, and delete internship offers
- View applicants
- Update application status:
  - Pending
  - Reviewed
  - Accepted
  - Rejected
- Recruiter dashboard

### Admin / School Features
- User management
- Offer moderation
- Platform monitoring
- Internship placement statistics
- Market demand overview

---

## AI & Smart Features

One of the key strengths of StageLink is the integration of a **small intelligent module**.

### 1. Internship Recommendation System
The platform recommends internships based on:

- student skills
- preferred city
- internship domain
- profile level

### 2. Explainable Match Score
The system compares student data with internship requirements and returns a percentage score.

Example:
- Student skills: `PHP, MySQL, Laravel, React`
- Offer requirements: `PHP, Laravel, MySQL`
- Result: **85% match**

But instead of stopping there, StageLink also explains the score:
- matched skills
- missing skills
- matched preferences
- profile compatibility

### 3. Skill Gap Detection
The platform can show which important skills are missing for a selected offer.

Example:
- Required: `Laravel, MySQL, Docker`
- Student has: `Laravel, MySQL`
- Missing skill: `Docker`

### 4. Employability Support
This feature helps the student improve over time by:
- identifying weak points
- suggesting missing skills
- improving readiness for internships

### Example Matching Formula
```text
Match Score =
( matched_skills / required_skills ) * 70
+ city_match * 10
+ domain_match * 10
+ profile_level_match * 10
