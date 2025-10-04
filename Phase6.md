# Phase 6: User Interface Development 
This phase focused on designing the user interface for the Salesforce application to improve usability for Agents, Managers, and Admins. The main objective was to make data entry, reporting, and navigation intuitive while providing quick access to key operational metrics.

## 1️⃣ Lightning App Builder & Record Pages

**Implementation:**

- A dedicated **Insurance Policy Management App** was created using **Lightning App Builder**.
- Custom **record pages** were configured for objects: Customer, Policy, Claim, and Agent/Mentor.
- Pages were designed to include relevant fields, related lists, and components for easy access.

**Procedure:**

1. Navigate to **Setup → App Builder → New Lightning App**.
2. Name the app: `Insurance Policy Management`.
3. Configure navigation: Add standard and custom tabs for Customers, Policies, Claims.
4. Customize record pages: **Setup → Object Manager → Select Object → Lightning Record Pages → Edit**.
5. Add sections and related lists to show linked records (e.g., Customer → Policies → Claims).

**Purpose:**

- Provides a structured and role-based UI for different users.
- Ensures agents and managers can access the most relevant data efficiently.

## 2️⃣ Tabs & Home Page Layouts

**Implementation:**

- Custom tabs were created for key objects to simplify navigation.
- Home page layout was configured to include dashboards and key metrics.

**Procedure:**

1. **Setup → Tabs → New → Select object → Name tab → Assign tab style.**
2. **Setup → Home Page Layouts → Edit → Add dashboard components and key reports.**

**Purpose:**

- Quick access to important modules and metrics.
- Improves productivity by reducing clicks and navigation time.
