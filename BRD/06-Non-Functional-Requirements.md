# 6. Non-Functional Requirements

This section defines the **quality attributes** essential for the AI-powered onboarding solution.  
They ensure performance, reliability, and compliance beyond functional features.

---

## 6.1 Performance
- System should process **KYC verification within 10 minutes** (target SLA).  
- OCR extraction accuracy must be at least **95%** for Aadhaar/PAN.  
- Face recognition match confidence should be **≥ 98%**.  

---

## 6.2 Scalability
- Solution must support onboarding **up to 1 million customers per month**.  
- Auto-scaling cloud infrastructure should handle seasonal spikes (e.g., tax season, festival campaigns).  

---

## 6.3 Security
- Data encryption **at rest (AES-256)** and **in transit (TLS 1.3)**.  
- Multi-factor authentication (MFA) for admin dashboards.  
- Adhere to **Zero Trust Architecture** principles.  

---

## 6.4 Compliance
- Align with **RBI, SEBI, and UIDAI** regulations.  
- Data residency: All PII stored in **India-based servers** (per RBI guidelines).  
- GDPR-like consent mechanism for international customers.  

---

## 6.5 Usability
- Mobile app designed for **multilingual support** (English, Hindi, Regional).  
- Average onboarding flow must be **< 5 minutes** for digitally literate users.  
- Error messages must be simple, non-technical, and assistive.  

---

## 6.6 Reliability
- **99.9% uptime SLA** for critical services.  
- Recovery Time Objective (RTO): < 1 hour.  
- Recovery Point Objective (RPO): < 15 minutes.  

---

These **Non-Functional Requirements (NFRs)** ensure that the onboarding solution is **secure, scalable, compliant, and user-friendly**, following enterprise standards used by consulting leaders like Deloitte and Genpact.
