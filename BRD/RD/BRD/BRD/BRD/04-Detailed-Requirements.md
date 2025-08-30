4. Detailed Requirements
4.1 Functional Requirements (What the System Must Do)

FR-1: Document Capture & Verification

System shall allow upload/capture of Aadhaar, PAN, and Proof of Address.

OCR shall extract key fields (Name, DOB, Address, PAN).

AI shall validate extracted data against UIDAI/NSDL databases.

FR-2: Identity Verification

System shall perform face match between uploaded photo and Aadhaar/PAN image.

Liveness detection shall ensure applicant is a real person during V-CIP.

FR-3: Dropout Prediction & Intervention

AI shall monitor user interactions (e.g., time spent on steps, abandonment signals).

System shall trigger proactive nudges (reminders, chatbot prompt, simplified flow) if dropout risk is ≥70%.

FR-4: Compliance Validation

System shall auto-check data against RBI/UIDAI KYC rules.

All actions shall be logged with timestamp for audit.

FR-5: Customer Communication

System shall notify customer of onboarding progress in real-time (SMS/email/app).

Premium customers shall receive personalized status updates.

4.2 Non-Functional Requirements (How the System Must Perform)

Performance

Verification response time ≤ 30 seconds per document.

System must support 10,000 concurrent onboarding sessions.

Security & Compliance

All data encrypted at rest and in transit (AES-256, TLS 1.3).

Aadhaar/UIDAI consent framework must be adhered to.

Compliance logs must be tamper-proof and audit-ready.

Availability

System uptime must be ≥ 99.9%.

Failover to backup servers in ≤ 5 minutes.

Scalability

Should scale from 100K → 10M customers without performance degradation.

4.3 Business Rules & Decision Logic

Aadhaar XML/eKYC verification is mandatory for all customers.

PAN validation required for accounts > ₹50,000 balance.

Manual fallback permitted in ≤15% of cases (poor image quality, OCR errors).

Premium customers flagged in CRM must be routed to concierge onboarding flow.

4.4 Integration Requirements

UIDAI eKYC API → Aadhaar validation.

NSDL API → PAN verification.

Core Banking System (CBS) → Account creation.

CRM → Customer profile & segmentation.

Fraud Management System → Blacklist/AML screening.
