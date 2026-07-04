# WorkPilot AI Design

## Overview

WorkPilot AI is the core intelligence layer of the system.

It acts as an AI Employee that understands messages, decides actions, and interacts with backend systems.

---

## Core AI Role

The AI is NOT just a chatbot.

It must:

- Understand user intent
- Classify requests
- Generate responses
- Decide actions (reply or create ticket)
- Use knowledge base

---

## AI Workflow

### Step 1: Input Message

User sends message:

Example:
- "น้ำไม่ไหล"
- "ไฟดับ"
- "จองสนามแบด"

---

### Step 2: Intent Detection

AI classifies message into:

- Question
- Maintenance request
- Booking request
- Complaint
- General inquiry

---

### Step 3: Context Retrieval

AI retrieves relevant information from:

- Knowledge Base (PDF, rules)
- Past messages
- Company settings

---

### Step 4: Decision Making

AI decides:

- Reply only
OR
- Create ticket
OR
- Ask for more information

---

### Step 5: Action Execution

If needed, AI calls backend APIs:

- Create ticket
- Update ticket
- Notify staff

---

### Step 6: Response Generation

AI generates human-like response in Thai language:

- Polite
- Clear
- Short
- Action-oriented

---

## Example Flow

Input:
"น้ำไม่ไหล"

↓

AI Output:
Intent: Maintenance
Category: Water Issue

↓

Action:
Create Ticket

↓

Response:
"รับเรื่องแจ้งซ่อมน้ำไม่ไหลแล้วครับ หมายเลข Ticket #102"

---

## AI Decision Rules

### Rule 1
If issue is urgent → create ticket immediately

### Rule 2
If information is missing → ask follow-up question

### Rule 3
If question exists in knowledge base → answer directly

### Rule 4
If uncertain → escalate to human staff

---

## AI Memory

AI remembers:

- User name
- Past issues
- Building information
- Frequent problems

---

## AI Prompt Structure

System Prompt includes:

- Role definition
- Business rules
- Tone of communication
- Safety rules
- Action rules

---

## AI + System Integration

AI does NOT work alone.

It must interact with:

- Backend API
- Database
- Knowledge Base
- Notification System

---

## Key Principle

AI is a decision layer, not just a chat tool.

---

## Goal

To replace human receptionist and admin tasks with AI that can:

- Understand
- Decide
- Act
- Report
