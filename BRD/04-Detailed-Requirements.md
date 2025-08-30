# 4. Detailed Requirements

This section defines the **functional and business requirements** for the AI-powered onboarding system.

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
