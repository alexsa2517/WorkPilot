# WorkPilot Database Design

## Overview

This document defines the core database structure of WorkPilot.

It supports multi-company SaaS with AI-powered communication and ticketing.

---

## Core Concept

Each company (building/estate) has its own isolated data.

---

## Main Tables

## 1. Users

Stores system users (admin, staff, residents)

- id
- name
- email
- password_hash
- role (admin / staff / resident)
- company_id
- created_at

---

## 2. Companies

Represents each property management client

- id
- name
- address
- plan_type
- created_at

---

## 3. Messages

Stores all chat messages between users and AI

- id
- company_id
- user_id
- message_text
- sender_type (user / AI)
- created_at

---

## 4. Tickets

Core maintenance request system

- id
- company_id
- user_id
- title
- description
- category (electric / water / general / other)
- status (open / in_progress / done)
- assigned_to
- created_at
- updated_at

---

## 5. Knowledge Base

Stores documents for AI learning

- id
- company_id
- title
- content
- file_type (pdf / text / url)
- created_at

---

## 6. AI Logs

Tracks AI decisions for debugging

- id
- company_id
- message_id
- intent_detected
- response_generated
- created_at

---

## 7. Notifications

Tracks all system notifications

- id
- company_id
- type (line / email)
- message
- status (sent / failed)
- created_at

---

## Relationships

- Company → Users (1 to many)
- Company → Messages (1 to many)
- Company → Tickets (1 to many)
- Company → Knowledge Base (1 to many)

---

## Key Principle

All data must be separated by company_id to support multi-tenant SaaS.

---

## Why This Design Works

- Scalable for thousands of buildings
- Supports AI + human workflow
- Easy to extend for new AI Employees

---

## Future Extensions

- Payments table
- Subscription table
- AI memory table
- Audit logs
