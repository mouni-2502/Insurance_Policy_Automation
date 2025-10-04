# Phase 8: Data Management & Backup

This phase focused on managing data within the Salesforce Developer Org for the Insurance Claim & Policy Management System. The goal was to ensure accurate records for Customers, Policies, Claims, and Mentors/Agents while maintaining data integrity.

---

## 1. Data Import & Record Creation

**Purpose:**  
Populate the system with sample data for testing and validation.

**Implementation:**  
- Sample Customers, Policies, and Claims were created manually through the Salesforce UI.  
- Ensured that records are linked correctly via lookup and master-detail relationships.

**Procedure:**  
1. Navigate to **Object Manager → Select Object** (e.g., Customer, Policy, Claim).  
2. Click **New** to create records.  
3. Fill in all required fields ensuring consistency in relationships.  
4. Save records and validate that relationships appear correctly in related lists.

---

## 2. Duplicate Management

**Purpose:**  
Prevent duplicate entries for Customers and Policies.

**Implementation:**  
- Unique fields such as **Customer Email** and **Policy Number** ensured data uniqueness.

**Procedure:**  
1. While creating new records, system enforced uniqueness of key fields.  
2. Manual verification ensured no duplicates existed in test data.

---

## 3. Data Backup (Manual)

**Purpose:**  
Maintain a backup of sample data within the org.

**Implementation:**  
- Exported records using **Reports** to Excel for reference.  
- Backup allowed verification of test data before proceeding to automation or reporting phases.

**Procedure:**  
1. Create a report for the object (e.g., Customers, Policies, Claims).  
2. Include all relevant fields.  
3. Click **Export → Excel Format** to save a local copy.
