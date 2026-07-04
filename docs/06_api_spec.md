# WorkPilot API Specification

## Overview

This document defines all core APIs for WorkPilot backend system.

It enables communication between frontend, backend, and AI engine.

---

## Authentication APIs

### Login

POST /api/auth/login

Request:
```json
{
  "email": "string",
  "password": "string"
}
