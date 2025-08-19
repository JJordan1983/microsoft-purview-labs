# Lab 01 – Compliance Administrator Role Validation

## 1. Role Overview
- **Role Name:** Compliance Administrator  
- **Assigned User:** Sarah Johnson  
- **Expected Permissions:**  
  - ✅ Create and manage DLP policies  
  - ✅ Configure compliance portal policies  
 

---

## 2. Lab Setup
- **Portal Used:** Microsoft Purview Compliance Portal  
- **Login Account:** Sarah.Johnson@domain.com  
- **Licenses Assigned:** Microsoft 365 E3  
- **Initial Access Test:** Login successful ✅  

---

## 3. Test Scenarios

### Scenario 1: Create a DLP Policy for Credit Card Numbers
**Steps Taken**
1. Navigated to **Compliance Portal → Data Loss Prevention → Policies → Create policy**  
2. Selected **Financial → U.S. Credit Card Numbers**  
3. Set policy mode to **Test with notifications**  
4. Sent a test email containing a U.S. credit card number  

**Result**  
- Triggered policy: ✅ Yes  
- Notification shown: ✅ Yes  

---

## 4. Enforce & Validate
- **Mode Change:** Switched from **Test** → **Enforce**  
- **Validation Action:** Sent another test email with a U.S. credit card number  
- **Result:** Email was **blocked successfully** ✅  


---

## 5. Observations & Issues
- Policy worked as expected in both **Test** and **Enforce** modes.  
- No critical errors encountered.  
- System correctly prevented restricted tasks outside of role permissions.  

---

## 6. Final Outcome
- **Role Function Verified?** ✅ Yes  
- **Key Evidence:**  
  - DLP block notification screenshot
  - <img width="1453" height="815" alt="image" src="https://github.com/user-attachments/assets/954b9fab-dc49-4d2d-826f-df1abae54f8a" />

  - <img width="811" height="586" alt="image" src="https://github.com/user-attachments/assets/eb5652ee-bafa-48d4-acaa-85874b49109a" />


- **Lab Status:** ✅ Complete  

---

🔒 This lab confirms that the **Compliance Administrator role** is properly scoped to manage DLP policies in Microsoft Purview while restricting higher-privilege directory tasks.
