# WorkPilot System Architecture

## Overview

WorkPilot is an AI-powered SaaS platform that automates communication and task management for property management companies.

---

## High-Level Architecture

User (Resident / Staff)
        ↓
Frontend (Web / Chat Interface)
        ↓
Backend API
        ↓
AI Engine (LLM + Prompt System)
        ↓
Database + Knowledge Base
        ↓
Notification System (LINE / Email)

---

## Core Components

### 1. Frontend
- Web application
- Chat interface for residents
- Admin dashboard for staff

---

### 2. Backend API
Handles all business logic:

- Authentication
- Chat processing
- Ticket creation
- Data management

---

### 3. AI Engine

Core intelligence of WorkPilot:

- Understand user messages
- Classify intent
- Generate responses
- Decide when to create tickets

Uses:
- LLM (Large Language Model)
- Prompt templates
- Context from Knowledge Base

---

### 4. Database

Stores:

- Users
- Companies
- Messages
- Tickets
- Knowledge base
- Logs

---

### 5. Knowledge Base

- PDF documents
- Rules and regulations
- Frequently asked questions

Used by AI for answering questions.

---

### 6. Ticket System

Workflow:

1. Resident reports issue
2. AI detects issue type
3. Ticket is created
4. Assigned to staff
5. Status is tracked

---

### 7. Notification System

Sends real-time alerts via:

- LINE
- Email
- Dashboard alerts

---

## Data Flow Example

Resident message:
"น้ำไม่ไหล"

↓

AI Engine:
Detects → Maintenance Issue

↓

Backend:
Creates ticket

↓

Database:
Stores ticket

↓

Notification:
Sends alert to staff

---

## Key Principle

AI does NOT replace the system.

AI works WITH the system:

- AI understands
- System executes
- Database stores
- Notification informs

---

## Scalability

System is designed to support:

- Multiple buildings
- Multiple companies
- Thousands of residents
- High message volume

---

## Summary

WorkPilot is:

AI + Backend + Database + Ticket System + Notification Layer

working together as one unified platform.
