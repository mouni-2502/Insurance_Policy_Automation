# 🧩 Phase 6: User Interface Development

This phase focused on designing and customizing the user interface of the **Insurance Policy Automation System** to make navigation simpler and record management more efficient for users such as **Agents, Managers, and Admins**.

The major UI components implemented in this project include:
- Custom Tabs  
- App Creation  
- Page Layouts for various custom objects  

---

## 🔹 1️⃣ App Creation – “Insurance Policy Management”

### 🎯 Purpose:
To provide a centralized workspace that contains all the relevant objects (**Customer, Policy, Claim, and Mentor**) under a single app for smooth operation and better accessibility.

### 🛠️ Implementation Steps:
1. Navigate to **Setup → App Manager → New Lightning App**  
2. Click **New Lightning App** and fill in the details:  
   - **App Name:** Insurance Policy Management  
   - **Developer Name:** Insurance_Policy_Management  
3. Select **Navigation Style:** Standard Navigation  
4. Add **Navigation Items (Tabs):**
   - Home  
   - Customer  
   - Policy  
   - Claim  
   - Mentor  
5. Assign the app to the required user profiles (**System Administrator, Standard User**)  
6. Click **Finish** to create and launch the app  

### ✅ Outcome:
A custom **Insurance Policy Management App** was successfully created, allowing users to access all modules in one place and switch easily between **Customers**, **Policies**, and **Claims**.

---

## 🔹 2️⃣ Custom Tabs Creation

### 🎯 Purpose:
Tabs help users navigate directly to different records or modules such as **Customer**, **Policy**, **Claim**, and **Mentor**.

### 🛠️ Implementation Steps:
1. Go to **Setup → Tabs → New**  
2. Choose **Custom Object Tab**  
3. Select the desired custom object (e.g., **Customer**)  
4. Enter the **Tab Label** and select a **Tab Style** (icon and color)  
5. Repeat the process for all required objects:
   - Customer  
   - Policy  
   - Claim  
   - Mentor  
6. Add these tabs to the **Insurance Policy Management App** navigation bar  

### ✅ Outcome:
All main entities of the project were made easily accessible through navigation tabs.  
This helped users manage **Customers**, **Policies**, and **Claims** efficiently.
<img width="1919" height="881" alt="Screenshot 2025-10-05 094603" src="https://github.com/user-attachments/assets/f44665c6-9e28-4854-b708-1c28368dfc7b" />

---

## 🔹 3️⃣ Page Layout Customization

### 🎯 Purpose:
To display only the relevant fields and related lists for each object, ensuring that data entry and record viewing are simple and organized.

### 🛠️ Implementation Steps:
1. Navigate to **Setup → Object Manager → Select Object (e.g., Policy)**  
2. Click **Page Layouts → Edit** (or create a new layout)  
3. Add or arrange required fields:  
   - **For Customer:** Name, Email, Contact Number, Address  
   - **For Policy:** Policy Number, Type, Premium, Coverage Amount, Start & End Dates  
   - **For Claim:** Claim Type, Amount, Status, Submission Date  
4. Add **Related Lists** (e.g., Customer → Policies → Claims) for linked data visibility  
5. Save the layout and assign it to the appropriate profiles  

### ✅ Outcome:
Customized **Page Layouts** were created for each custom object, ensuring a clean, user-friendly interface with relevant data displayed efficiently.
<img width="1890" height="777" alt="Screenshot 2025-10-05 100001" src="https://github.com/user-attachments/assets/3c5e72fc-b84c-4790-ac29-0bb1caa9fcd6" />
<img width="1902" height="778" alt="Screenshot 2025-10-05 095911" src="https://github.com/user-attachments/assets/3ef31f5b-79ae-484c-b419-8910098be409" />
<img width="1902" height="779" alt="Screenshot 2025-10-05 100044" src="https://github.com/user-attachments/assets/02c759c1-8fc5-4fea-8456-774e362cc38f" />



---
