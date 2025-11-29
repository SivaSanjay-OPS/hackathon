# LoanSphere — Loan Issuance & Document Review System (Frontend-Only SPA)

LoanSphere is a **complete front-end loan management system** built as a  
single-page application (SPA) using **HTML, CSS, JavaScript**, with:

- Lender Dashboard  
- Borrower Dashboard  
- Admin Dashboard  
- Analyst Dashboard  
- HR Dashboard  

It supports **loan issuance, EMI calculation, document upload & verification,  
credit scoring, payment tracking, reports, CSV exports**, and **localStorage  
persistence**. The application is designed to satisfy **Y24-SDC rubric  
requirements** for UI/UX, routing, validation, CRUD, persistence, API  
integration (pluggable), role management, and code understanding.

---

## 📌 Project Highlights

### 🔹 Multi-Role Dashboards (all in one SPA)
- Dashboard (overview metrics + recent loans + pending docs)
- Lender (offers, marketplace publishing)
- Borrower (plans, apply, upload documents, loan schedule & EMI)
- Admin (document review, user oversight)
- Analyst (charts + CSV export)
- HR (role assignment and user removal)

### 🔹 Loan Processing Features
- EMI formula implementation  
- Full amortization schedule  
- Transaction logs for each payment  
- Admin workflow for document verification  
- Borrower credit score simulation  

### 🔹 Document Workflow
Borrowers upload PDF/JPG/PNG → Stored in Base64 → Added to pending queue →  
Admin accepts/rejects with reason → Status stored.

### 🔹 Data Storage (Frontend Only)
- All data uses `localStorage` via `DB.get`, `DB.set`, `DB.add`
- Keys: `offers`, `market`, `loans`, `users`, `pendingDocs`,  
  `reviewedDocs`, `transactions`

### 🔹 Pluggable API Layer (Fetch/Axios Ready)
`USE_API = false` uses localStorage.  
Set `USE_API = true` to automatically send requests to  
`API_BASE + '/entity'`.

---

# 📁 Folder Structure

