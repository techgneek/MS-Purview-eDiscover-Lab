## 🔍 Microsoft Purview Lab – eDiscovery Setup & Search Lab

### 🎯 Scenario: Internal HR Investigation for Payroll Keyword

Your organization’s HR department has received a whistleblower report suggesting confidential payroll information may have been mishandled via internal emails and files. As part of the security and compliance team, you’ve been tasked with using **Microsoft Purview eDiscovery (Standard)** to identify any data related to the keyword **"payroll"** in **Exchange mailboxes**, **SharePoint sites**, and **public folders**.

---

## ✅ Lab Objective

Use Microsoft Purview eDiscovery to:

* Create a case for investigation
* Run a content search using the keyword **"payroll"**
* Scope the search to Exchange, SharePoint, and Public Folders
* Save and monitor the search progress

---

## 🧪 Step-by-Step Instructions

### **🧱 Step 1: Create an eDiscovery Case**

* Go to **Microsoft Purview > eDiscovery (Standard)**
* Click **Create a Case**
* Name it something relevant (e.g., `FirstCase`)
* Status will show as **Active**

📸 `Step 1 - Create Case`
<img width="1650" alt="Screen Shot 2025-05-19 at 7 24 40 PM" src="https://github.com/user-attachments/assets/18643f3e-5e25-4157-8b39-f6df97b80567" />

---

### **📝 Step 2: Add a Search to the Case**

* Inside the case, navigate to the **Searches** tab
* Click **+ New search**
* Name the search (e.g., `Search1`)
* Add a description like “Searching for payroll-related content”

📸 `Step 2 - Add Search Name
<img width="1777" alt="Screen Shot 2025-05-19 at 7 25 34 PM" src="https://github.com/user-attachments/assets/cbad754c-befc-4655-b591-3b0aa831a4e3" />

---

### **🌐 Step 3: Define Search Locations**

* Toggle ON:

  * **Exchange mailboxes**
  * **SharePoint sites**
  * **Exchange public folders**
* Optionally, check “Add App Content for On-Premises Users”

📸 `Step 3 - Define Locations`
<img width="1733" alt="Screen Shot 2025-05-19 at 7 26 03 PM" src="https://github.com/user-attachments/assets/aa40720f-65e7-4d79-bb15-881ce43365e5" />

---

### **🔍 Step 4: Add Search Conditions**

* Choose **Query Builder**
* Under **Keywords**, enter:

  ```
  payroll
  ```

📸 `Step 4 - Define Conditions`
<img width="1733" alt="Screen Shot 2025-05-19 at 7 26 49 PM" src="https://github.com/user-attachments/assets/4c429376-5004-4970-85b8-2d5c2c071e95" />

---

### **📋 Step 5: Review and Create the Search**

* Review:

  * Name: `Search1`
  * Criteria: `payroll`
  * Locations: Exchange, SharePoint, Public Folders
* Click **Submit**

📸 `Step 5 - Review & Submit`
<img width="1733" alt="Screen Shot 2025-05-19 at 7 27 04 PM" src="https://github.com/user-attachments/assets/c5f2eb28-2d13-4205-a1be-dd97881c617a" />

---

### **⏱️ Step 6: Monitor the Search**

* Go back to the **Searches** tab
* Monitor status: "Starting" ➝ "Completed"
* No export is needed unless analysis is required externally

📸 `Step 6 - Monitor Search`
<img width="1733" alt="Screen Shot 2025-05-19 at 7 29 31 PM" src="https://github.com/user-attachments/assets/1e93b0aa-06ec-4f86-8072-a64cf70fa002" />

---

## 📌 Notes

* This lab aligns with **NIST 800-53 AU-6 (Audit Review, Analysis, and Reporting)** and **IR-4 (Incident Handling)** for evidence collection and internal investigation.
* Microsoft Purview helps ensure regulatory compliance (e.g., HIPAA, GDPR, PCI DSS) by enabling data searches and holds.
