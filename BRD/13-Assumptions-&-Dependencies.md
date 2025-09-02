# 13. Assumptions & Dependencies

This section documents the **assumptions** made during the planning of the AI-powered customer onboarding project and the **dependencies** that could impact delivery.


| ID   | Assumption / Dependency                        | Description                                                                 |
|------|------------------------------------------------|-----------------------------------------------------------------------------|
| A-1  | Reliable internet connectivity                  | Smooth customer onboarding depends on stable mobile and broadband networks. |
| A-2  | Access to UIDAI and regulatory APIs             | Aadhaar e-KYC and PAN validation require uninterrupted access to govt APIs. |
| A-3  | Customer device compatibility                   | AI-powered verification assumes customers use smartphones with camera & internet. |
| A-4  | Timely integration with core banking systems    | Future state onboarding depends on APIs being available and responsive.     |
| A-5  | Regular dataset availability for AI model training | Continuous access to updated KYC and fraud datasets is required.           |


## Assumptions
1. Regulatory guidelines (RBI, SEBI, IRDAI) will remain stable during the project timeline.  
2. Customers will have access to smartphones and internet connectivity for digital onboarding.  
3. Adequate training and change management support will be available for staff adoption.  
4. AI/ML models will achieve acceptable accuracy levels (>95%) after training.  
5. Partner APIs (Aadhaar, PAN, CKYC, credit bureaus) will remain available and functional.  

---

## Dependencies
1. **Third-Party Vendors**  
   - Reliance on OCR, liveness detection, and fraud detection vendors for core AI capabilities.  

2. **Regulatory Bodies**  
   - RBI/UIDAI approvals and compliance checks.  

3. **Technology Infrastructure**  
   - Dependence on cloud platforms (AWS, Azure, GCP) for hosting and scaling AI workloads.  

4. **Data Availability**  
   - Access to clean, reliable, and diverse customer data for training AI models.  

5. **Integration with Core Banking Systems**  
   - Seamless API connectivity and support from internal IT teams.  

---

## Monitoring Approach
- Maintain an **Assumption & Dependency Log**.  
- Review items at **Steering Committee meetings**.  
- Escalate critical risks to senior stakeholders in advance.  

---

✅ Capturing these assumptions and dependencies provides **clarity and transparency**, reducing uncertainty and strengthening delivery confidence.
