#  🔐NyayaVault – Secure Digital Document Management System

## SIH26-26190

NyayaVault is a **Secure Digital Document Management System** designed to securely store, organize, search, and manage legal and police-related documents in one centralized platform.

It helps manage documents such as:

* FIRs
* Police Reports
* Witness Statements
* Charge Sheets
* Evidence Documents
* Forensic Reports
* Court Filings
* Judgments

The system focuses on **secure document storage, smart search, access control, and audit tracking**.

---

## Key Features

### 🔐 Secure Document Management

* Centralized storage for legal documents
* Controlled access to sensitive documents
* Organized document categories

### 🔎 Smart Search

* Search old FIRs and legal records
* Quickly locate required documents
* Search using document details and keywords

### 👥 Role-Based Access

Different users can have different permissions based on their role.

Example roles:

* Admin
* Police Officer
* Court Staff
* Authorized User

### 📋 Audit Trail

The system keeps track of important actions such as:

* Document upload
* Document access
* Document modification
* Document deletion

### 📁 Document Organization

Documents can be organized according to their type, case, and related information.

---

## Technology Stack

### Frontend

* React
* TypeScript
* Vite

### Backend

* Node.js
* Express.js
* TypeScript

### Database

* PostgreSQL
* Drizzle ORM

### Other Technologies

* Zod
* Orval
* REST API

---

## Project Structure

```text
nyayavault-full-source/
│
├── artifacts/
│   ├── nyayavault/          # Frontend
│   └── api-server/          # Backend
│
├── lib/
│
├── package.json
├── pnpm-lock.yaml
├── replit.md
└── README.md
```

---

# Installation and Execution

## Prerequisites

Install the following before running the project:

* Node.js
* pnpm
* PostgreSQL

Check Node.js:

```bash
node --version
```

Check pnpm:

```bash
pnpm --version
```

---

## 1. Clone the Repository

```bash
git clone YOUR_GITHUB_REPOSITORY_URL
```

Go to the project folder:

```bash
cd nyayavault-full-source
```

---

## 2. Install Dependencies

```bash
pnpm install
```

---

## 3. Configure Environment Variables

Create a `.env` file for the backend.

Add:

```env
DATABASE_URL=your_postgresql_database_url
PORT=5000
```

Replace the database URL with your PostgreSQL connection string.

---

## 4. Start the Backend

Open a terminal in the project root and run:

```bash
pnpm --filter @workspace/api-server run dev
```

The backend will run on:

```text
http://localhost:5000
```

---

## 5. Start the Frontend

Open **another terminal** in the same project folder.

Run:

```bash
pnpm --filter @workspace/nyayavault run dev
```

The frontend will normally run on:

```text
http://localhost:5173
```

---

## 6. Open the Application

Open your browser and visit:

```text
http://localhost:5173
```

The NyayaVault application should now be available.

---

## API

Backend API:

```text
http://localhost:5000
```

The backend provides APIs required by the NyayaVault frontend for document and application functionality.

---

## Security Focus

NyayaVault is designed around the following security concepts:

* Authentication
* Role-based access control
* Controlled document access
* Secure document storage
* Audit logging
* Protection of sensitive legal records

---

## Problem Statement

### SIH26-26190 – Secure Digital Document Management System

Police departments and courts handle a large number of important digital documents. These documents can become difficult to manage when they are stored across different locations and systems.

NyayaVault provides a centralized system where authorized users can securely manage legal documents, search historical records, organize case information, and track document-related activities.

---

## Future Enhancements

* Advanced AI-powered document search
* OCR for scanned documents
* Automatic document classification
* Digital signatures
* Advanced encryption
* Document version history
* Evidence chain-of-custody tracking
* Advanced analytics and dashboards

---

## Disclaimer

This project is developed as a **prototype for the Smart India Hackathon (SIH26)** problem statement SIH26-26190.

It is intended for demonstration and educational purposes and is not a production-ready government legal-record system.

---

## Project

**Project Name:** NyayaVault
**Problem Statement:** SIH26-26190
**Category:** Secure Digital Document Management System
