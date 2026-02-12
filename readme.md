# FieldSewa – Smart Employee Field Tracking System

> Real-time GPS-based employee field tracking and task management system built with Flutter & Firebase.

## TL;DR

FieldSewa is a role-based workforce management system where:

- Admin creates Managers and Employees  
- Manager assigns field tasks  
- Employee completes tasks with GPS validation  

✔ Real-time tracking  
✔ Secure authentication  
✔ Cloud-based system  
✔ Role-based control  

## Team
| Name               | Role / Contribution           | 
|--------------------|-------------------------------|
| Riya Maharjhan     | System Design & Backend Logic |
| Raj Kumar Jha      | Flutter Development           |
| Dipen Niraula      | UI/UX & Integration           |
| Mandip Dhungana    | Testing & Documentation       |

**Technology Used:** Flutter + Firebase  
**Project Type:** Mobile Application  

---

## Problem Statement

Organizations with field employees (banks, insurance agents, sales teams, delivery staff) face:

-  Fake check-ins  
-  No real-time visibility  
-  Manual reporting delays  
-  Lack of accountability  
-  Travel claim fraud  

Existing solutions are often expensive and overly complex.

---

## Solution Overview

FieldSewa provides a secure and structured employee tracking system with three user roles:

### Admin
- Creates Manager accounts
- Creates Employee accounts
- Monitors system overview

### Manager
- Creates field tasks
- Assigns tasks to employees
- Monitors task progress
- Reviews completion reports

### Employee
- Views assigned tasks
- Starts task with GPS validation
- Updates task status
- Submits completion report

---

## Key Features

- Role-Based Authentication (Admin / Manager / Employee)
- Firebase Authentication
- Cloud Firestore Database
- GPS Location Verification
- Task Assignment System
- Real-Time Status Updates
- Secure Cloud Storage
- Clean & Responsive Flutter UI

## Screenshots


## Architecture OverView
Diagram:

### 🔄 Flow

User (Flutter App)  
→ Firebase Authentication  
→ Cloud Firestore  
→ Real-Time Sync  
→ UI Update  

### Components

- **Frontend:** Flutter
- **Backend Services:** Firebase
- **Database:** Cloud Firestore
- **Authentication:** Firebase Auth
- **Location Service:** GPS (Flutter location package)

## Firestore Data Structure (Sample)

users/
userId
- name
- email
- role (admin/manager/employee)
- createdBy

tasks/
taskId
- title
- description
- assignedTo
- createdBy
- status (pending/in-progress/completed)
- startLocation
- completionReport
- timestamp

---

## Security & Privacy

FieldSewa ensures:

- Firebase Authentication
- Role-based access control
- Firestore security rules
- Encrypted HTTPS communication
- GPS validation before task start
-  No tracking outside working hours


##  Anti-GPS Manipulation Strategy

- Mock location detection (device level)
- Backend coordinate validation
- Sudden location jump detection
- Distance-time speed calculation
- Future: Play Integrity API integration

---

## ⚙ Setup Instructions

### 1️⃣ Prerequisites

- Flutter SDK
- Firebase Account
- Android Studio / VS Code

---

### 2️⃣ Clone Repository

```bash
git clone <repository-url>
cd FieldSewa

3️⃣ Install Dependencies
- flutter pub get

4️⃣ Firebase Setup
- Create Firebase Project
- Enable Authentication (Email/Password)
- Enable Cloud Firestore
- Download google-services.json
- Place inside android/app/

5️⃣ Run the App
- flutter run

### Usage Walkthrough
-Login as Admin
-Create Manager account
-Create Employee account
-Login as Manager
-Create and assign task
-Login as Employee
-Start task (GPS verified)
-Complete task and submit report
-Manager views report

### Future Scope
-Admin Analytics Dashboard
-AI Productivity Insights
-Route Optimization
-Push Notifications
-Offline Mode with Sync
-Flutter Web Version
-Development Timeline

###Timeline (Hackathon Log)
Day 1
System design
Firebase setup
Role-based authentication

Day 2
Task management system
Firestore integration
UI implementation

Day 3
GPS validation
Security rules
Testing & bug fixing

# Credits & License
## Project Name:FieldSewa
## Author: Team Infyrus
## Year: 2026

## License

© 2026 fieldSewa

**Demo-Only License**  

Permission is granted to **view and use this software only for demonstration purposes**.  
**Modification, redistribution, or transfer of ownership is strictly prohibited** without explicit permission from the copyright holder.  

**Notes on included assets / libraries / datasets:**  
- Any third-party datasets, APIs, or assets retain their original licenses.  
- Users must comply with those licenses if they access or use the resources separately.
