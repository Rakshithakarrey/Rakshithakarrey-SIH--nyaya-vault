# 🔐 NyayaVault — Secure Digital Document Management System

NyayaVault is a **Secure Digital Document Management System** designed for managing sensitive legal and investigation-related documents in a centralized and organized environment.

The project is developed as a prototype for **Smart India Hackathon (SIH26)** problem statement **SIH26-26190 – Secure Digital Document Management System**.

It focuses on secure document storage, role-based access, document organization, searching, and audit tracking.

---

## 🎯 Problem Statement

Police departments, forensic laboratories, prosecution offices, and courts handle a large number of digital documents such as:

* FIRs
* Police reports
* Witness statements
* Charge sheets
* Evidence records
* Forensic reports
* Court filings
* Judgments

Managing these documents across different systems can make it difficult to locate information quickly and maintain proper access control.

### 💡 Proposed Solution

NyayaVault provides a centralized digital workspace where authorized users can:

* Upload legal documents
* Organize documents by case and category
* Search documents quickly
* Control access according to user roles
* Track document activities
* Maintain an audit trail
* Manage case-related records securely

---

## 🚀 Key Features

### 📁 1. Digital Case File Management

Documents can be organized according to cases and document categories.

Examples:

* FIR
* Evidence
* Forensic Report
* Charge Sheet
* Witness Statement
* Court Document

### 🔎 2. Smart Document Search

Users can search for documents using relevant information such as:

* Case ID
* Document name
* Document type
* Keywords
* Date

### 🔐 3. Role-Based Access Control

Different users can have different permissions.

Example roles:

| Role                  | Example Access                 |
| --------------------- | ------------------------------ |
| Administrator         | Manage users and system        |
| Investigating Officer | Manage investigation documents |
| Forensic Expert       | Manage forensic documents      |
| Prosecutor            | Review prosecution documents   |
| Judge                 | Review court documents         |
| Auditor               | Review audit activities        |

### 📝 4. Audit Trail

Important document activities can be recorded, such as:

* Upload
* View
* Download
* Update
* Permission changes
* Document access

This helps provide accountability for document activity.

### 🛡️ 5. Secure Document Management

The system is designed to restrict unauthorized access to sensitive legal records through authentication and role-based permissions.

### 📊 6. Case Organization

Documents can be associated with particular cases so that users can access the relevant case information from a centralized workspace.

---

## 🏗️ System Architecture

```text
                 ┌─────────────────────┐
                 │       User          │
                 │ Police / Court /    │
                 │ Forensic / Auditor  │
                 └──────────┬──────────┘
                            │
                            ▼
                 ┌─────────────────────┐
                 │     Frontend        │
                 │   React + Vite      │
                 └──────────┬──────────┘
                            │
                            ▼
                 ┌─────────────────────┐
                 │      Backend        │
                 │ Node.js + Express   │
                 └──────────┬──────────┘
                            │
                            ▼
                 ┌─────────────────────┐
                 │      Database       │
                 │ PostgreSQL / ORM    │
                 └─────────────────────┘
```

---

## 🛠️ Technology Stack

### Frontend

* React
* TypeScript
* Vite
* Tailwind CSS

### Backend

* Node.js
* Express.js
* TypeScript

### Database

* PostgreSQL
* Drizzle ORM

### API

* REST API
* Zod validation

### Development Tools

* Git
* GitHub
* VS Code
* pnpm

---

## 📂 Project Structure

```text
nyayavault-full-source/
│
├── artifacts/
│   ├── nyayavault/
│   │   └── frontend files
│   │
│   └── api-server/
│       └── backend files
│
├── lib/
│   └── shared libraries
│
├── package.json
├── pnpm-lock.yaml
├── pnpm-workspace.yaml
└── README.md
```

---

# 💻 Running the Project Locally

## 1. Prerequisites

Install:

* Node.js
* pnpm
* PostgreSQL

Check Node.js:

```powershell
node --version
```

Check pnpm:

```powershell
pnpm --version
```

---

## 2. Clone the Repository

```powershell
git clone YOUR_GITHUB_REPOSITORY_URL
```

Move into the project:

```powershell
cd nyayavault-full-source
```

---

## 3. Install Dependencies

```powershell
pnpm install
```

---

## 4. Configure Environment Variables

Create the required `.env` file for the backend.

Example:

```env
DATABASE_URL=your_postgresql_connection_string
PORT=5000
```

Do **not** upload real passwords, API keys, database credentials, or other secrets to GitHub.

---

## 5. Start the Backend

Open a terminal in the project directory and run:

```powershell
$env:PORT="5000"
pnpm --filter @workspace/api-server run dev
```

The backend should run on:

```text
http://localhost:5000
```

---

## 6. Start the Frontend

Open another terminal in the same project directory.

Run:

```powershell
$env:PORT="5173"
$env:BASE_PATH="/"
pnpm --filter @workspace/nyayavault run dev
```

The frontend should be available at:

```text
http://localhost:5173
```

> If port 5173 is already being used, stop the previous Vite process or use another available port.

---

# 🌐 Project Links

### GitHub Repository

**Your repository:**
`YOUR_GITHUB_REPOSITORY_URL`

### Live Demo

**Frontend:**
`YOUR_FRONTEND_URL`

### Backend API

**Backend:**
`YOUR_BACKEND_URL`

> Only add live deployment links after you have deployed your own application. Do not list another developer's deployment as your own.

---

# 🔒 Security Considerations

NyayaVault is designed around the security requirements of legal document management.

Important considerations include:

* Authentication
* Role-based authorization
* Protected document access
* Audit logging
* Secure database access
* Input validation
* Environment-based secret management

For a production deployment, additional security measures would be required, including infrastructure hardening, key management, encryption policies, backup and recovery procedures, monitoring, and formal security testing.

---

# 🎯 SIH26 Alignment

**Problem Statement:** SIH26-26190

**Title:** Secure Digital Document Management System

NyayaVault addresses the problem by providing a centralized platform for:

```text
Legal Documents
      ↓
Centralized Storage
      ↓
Case Organization
      ↓
Role-Based Access
      ↓
Document Search
      ↓
Audit Tracking
```

---

# 🔮 Future Enhancements

Potential future improvements include:

* Advanced OCR
* Semantic document search
* AI-assisted document classification
* Automated PII detection and redaction
* Digital signatures
* Cryptographic document verification
* QR-based document verification
* Advanced chain-of-custody tracking
* Multi-factor authentication
* Cloud deployment
* Automated backup and recovery

---

# 👩‍💻 Project

**NyayaVault**

Secure Digital Document Management System

Developed as a prototype for **Smart India Hackathon (SIH26)**.

---

## 📜 Disclaimer

NyayaVault is an academic/hackathon prototype. It is not intended to replace officially approved government, police, forensic, prosecution, or judicial systems.

Production use would require appropriate security audits, legal compliance reviews, infrastructure controls, and authorization from the relevant authorities.
