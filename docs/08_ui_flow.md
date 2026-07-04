# WorkPilot UI Flow

## Overview

This document describes how users interact with WorkPilot system through screens and navigation flow.

---

# 1. Login Flow

Login Page
   ↓
Enter Email / Password
   ↓
Dashboard

---

# 2. Main Dashboard Flow

Dashboard
   ↓
- Chat Messages
- Tickets
- Knowledge Base
- Settings

---

# 3. Resident Chat Flow

Chat Screen
   ↓
User sends message
   ↓
AI responds instantly
   ↓
If needed → Ticket created
   ↓
Show ticket number

---

# 4. Maintenance Ticket Flow

Resident reports issue
   ↓
AI detects problem
   ↓
Ticket created automatically
   ↓
Assigned to staff
   ↓
Staff updates status
   ↓
Ticket closed

---

# 5. Admin Flow

Admin Login
   ↓
Dashboard
   ↓
View all tickets
   ↓
Assign staff
   ↓
Track progress
   ↓
Generate reports

---

# 6. Knowledge Base Flow

Admin uploads file (PDF / text)
   ↓
System stores data
   ↓
AI uses data for answering questions

---

# 7. Notification Flow

System event occurs
   ↓
(e.g. new ticket created)
   ↓
Send notification
   ↓
LINE / Email / Dashboard alert

---

# 8. Multi-Tenant Flow

User logs in
   ↓
System checks company_id
   ↓
Loads only that company's data
   ↓
Prevents data mixing

---

# Key Principle

Every screen is connected to an action.

UI is not just design.
UI is a workflow system.

---

# Example End-to-End Flow

Resident:
"น้ำไม่ไหล"

↓

Chat Screen

↓

AI Response:
"รับเรื่องแล้ว"

↓

Ticket Created

↓

Admin Dashboard

↓

Staff Assigned

↓

Status Updated

↓

Notification Sent
