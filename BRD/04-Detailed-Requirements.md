# 4. Detailed Requirements

This section defines the **functional and business requirements** for the AI-powered onboarding system.

## Functional Requirements

| ID       | Requirement                  | Description |
|----------|------------------------------|-------------|
| FR-001   | User Authentication          | The system must allow customers to log in using username/password or supported SSO methods (e.g., Google, OTP). |
| FR-002   | Dashboard Access             | Upon login, users must be able to view a dashboard with onboarding status and available actions. |
| FR-003   | Document Upload              | The system must allow customers to upload ID documents (Aadhaar, PAN, Passport) in image/PDF format. |
| FR-004   | OCR Extraction               | The system must automatically extract customer details from uploaded documents using OCR with ≥95% accuracy. |
| FR-005   | Data Validation              | Extracted details must be validated against predefined rules (e.g., Aadhaar format, PAN checksum). |
| FR-006   | KYC Verification             | The system must verify uploaded documents against external KYC databases or APIs. |
| FR-007   | Validation Progress          | Customers must see real-time validation progress (Pending, In Progress, Completed, Failed). |
| FR-008   | Validation Result            | The system must display the final result (Approved/Rejected) with reasons for rejection if applicable. |
| FR-009   | Manual Review Escalation     | Cases failing automated checks must be escalated to a compliance team for manual review. |
| FR-010   | Notifications                | Users must receive real-time notifications (email/SMS/in-app) on onboarding status changes. |
| FR-011   | Admin Login                  | Admin users must be able to log in securely to the web portal with RBAC (Role-Based Access Control). |
| FR-012   | Admin Dashboard              | Admin users must view overall onboarding statistics, pending verifications, and flagged cases. |
| FR-013   | Case Management              | Admins must assign, review, and resolve escalated onboarding cases. |
| FR-014   | Reports & Audit Logs         | The system must generate audit logs of all onboarding activities and allow admins to export reports. |
| FR-015   | Data Encryption              | All uploaded documents and extracted data must be stored in encrypted format (AES-256). |
| FR-016   | Session Timeout              | The system must automatically log out users after a configurable period of inactivity. |
| FR-017   | Multi-Language Support       | The system must support multiple languages (at least English and Hindi) for customer onboarding. |
| FR-018   | Error Handling               | The system must provide clear error messages and recovery steps for failed uploads or validations. |
| FR-019   | Scalability                  | The system must handle concurrent onboarding requests (at least 10,000 users simultaneously). |
| FR-020   | Compliance Reporting         | The system must generate compliance-ready reports for audits (e.g., RBI/SEBI requirements). |


## 4.1 Functional Requirements
1. **Customer Registration**
   - Capture personal details via mobile/web app.
   - Validate email and mobile number with OTP.

2. **Document Upload & Verification**
   - Upload Aadhaar, PAN, and proof of address.
   - Auto-extract details using OCR.
   - Cross-check details with regulatory APIs (UIDAI, PAN services).

3. **Biometric & Liveness Detection**
   - Capture selfie video for real-time verification.
   - AI model validates match between ID and selfie.

4. **Fraud Detection**
   - Flag duplicate accounts using AI-driven anomaly detection.
   - Detect manipulated documents/images.

5. **Smart Nudges**
   - AI-driven chatbots guide users who stall during onboarding.
   - Contextual help messages (e.g., “Your PAN upload failed, please retry”).

6. **Compliance Checks**
   - Auto-check against CKYC and RBI watchlists.
   - Generate onboarding audit logs.

7. **Onboarding Completion**
   - Auto-generate digital account number.
   - Send confirmation via SMS/email.

---

## 4.2 Non-Functional Requirements (covered in detail later in Section 6)
- High system uptime (99.9% SLA).
- Secure data encryption at rest and in transit.
- Mobile responsiveness and accessibility standards.

---

## 4.3 Business Rules
- PAN and Aadhaar are mandatory for individual onboarding.  
- All document uploads must be under 5 MB, in JPEG/PNG/PDF.  
- Minimum age: 18 years.  
- One customer = one unique PAN (no duplicate accounts).  

---

## 4.4 User Stories
- **As a new customer**, I want to open an account in under 10 minutes so that I can start using banking services instantly.  
- **As a compliance officer**, I want a dashboard to track onboarding cases and flagged risks so that I can ensure regulatory compliance.  
- **As a product manager**, I want real-time analytics on dropout points so that I can improve the onboarding journey.  

---

This detailed requirements section ensures alignment between **business needs, compliance obligations, and technical capabilities**.
