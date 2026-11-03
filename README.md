# Quizora

**Quizora** is a full-stack online assessment and skill-evaluation platform built with **.NET 9** and **Clean Architecture**.  
It enables companies to create and manage technical tests, invite candidates, evaluate results, and support interview workflows—while candidates can practice, take mock tests, solve coding problems, and track performance.

---

## Overview

| Role | Capabilities |
|------|----------------|
| **Company** | Create tests, manage questions, invite candidates, view results, trigger interview calls |
| **Candidate** | Receive invitations, take tests, practice by category, attempt mock tests, solve coding problems, manage profile/CV |

---

## Features

### Authentication & Security
- JWT-based authentication with role-based authorization (Company / Candidate)
- Secure password hashing (BCrypt)
- Forgot Password & Reset Password via email (time-limited token)
- Profile management and password change

### Company Module
- Create and manage tests (duration, status, passing criteria)
- Add multiple-choice questions with options
- Invite candidates by email
- View candidate results and scores
- Interview invitation workflow with email notifications

### Candidate Module
- View and accept test invitations
- Take timed assessments and submit answers
- Automatic scoring and result summary
- Practice quizzes by category
- Mock tests with timed sessions
- Coding practice problems with submissions
- CV upload and profile management

### Additional Capabilities
- AI-assisted features (configurable AI provider)
- Notifications
- Contests
- Email notifications for results and interview calls

---

## Tech Stack

| Layer | Technology |
|-------|------------|
| **Backend API** | ASP.NET Core 9 Web API |
| **Frontend** | Blazor Server (.NET 9) |
| **Architecture** | Clean Architecture |
| **ORM** | Entity Framework Core |
| **Database** | PostgreSQL |
| **Auth** | JWT Bearer + BCrypt |
| **Validation** | FluentValidation |
| **Email** | SMTP (Gmail App Password supported) |
| **API Docs** | Swagger / OpenAPI |
| **Container** | Docker |
| **Deployment** | Render |

---

## Solution StructureQuizora/
├── Quizora.sln
└── src/
├── Quizora.API/
├── Quizora.Application/
├── Quizora.Domain/
├── Quizora.Infrastructure/
└── Quizora.Web/
