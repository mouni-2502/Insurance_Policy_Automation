# 📘 Insurance Claim & Policy Management System

## 1. Problem Statement
Insurance companies manage thousands of policies and claims, but traditional processes are often manual, time-consuming, and fragmented. Customers face delays in claim approvals, missed premium reminders, and limited visibility into policy or claim status. Agents struggle to manage customer portfolios efficiently, while managers lack real-time insights for decision-making and face challenges in detecting fraudulent claims.

To overcome these issues, a Salesforce CRM solution is required to automate policy issuance and renewals, streamline claim processing with multi-level approvals, provide customers with a transparent self-service portal, and deliver fraud detection alerts along with real-time dashboards for compliance and performance monitoring.

## Phase 2: Salesforce Org Setup
- Set up a Lightning Developer Org to design and implement all custom modules.  
- Enabled features required for the project:
  - Lightning Experience for UI customization
  - Reports and Dashboards for monitoring KPIs
  - Workflow Rules and Approval Processes for automation
- Configured org settings to support multi-user roles and permissions.

## Phase 3: Custom Object Creation
- Created custom objects to manage the data efficiently:
  - **Customers:** Captures personal details and links with policies and claims.
  - **Policies:** Stores policy information including number, type, coverage, premium, and customer association.
  - **Claims:** Tracks claim submission, type, amount, status, and associated policy.
  - **Mentors/Agents:** Maintains agent/mentor records and links them to assigned customers.
- Each object was configured with necessary fields, page layouts, and relationships for proper data handling.

## Phase 4: Object Relationships
- Designed lookup relationships to connect objects:
  - **Customer → Policies & Claims** for complete customer tracking
  - **Mentor → Customer** to assign agents for customer guidance
- Ensured related lists on Lightning pages display all connected records for ease of use.  
- Relationships improve data integrity and traceability, enabling efficient reporting and approvals.

## Phase 5: Role-Based Access & Permissions
- Defined profiles: Admin, Agent, Manager  
- **Admin:** Full access to all objects and fields  
- **Agents/Managers:** Limited access to assigned records  
- Implemented field-level security for sensitive information such as claim amounts and customer contact details.  
- Ensured security and compliance, allowing only authorized users to access or modify data.

## Phase 6: Workflow Automation
- Implemented workflow rules to automate repetitive tasks:
  - Notify managers of pending claims to ensure timely approvals
  - Send automatic policy renewal reminders to customers
- Automation helps reduce manual errors, improves efficiency, and ensures timely follow-ups.

## Phase 7: Approval Processes
- Designed multi-level claim approval workflow:
  - **Submitted → Agent → Manager**
- Each stage triggers email notifications, ensuring stakeholders are informed.  
- Claims are tracked through statuses: **Submitted → Approved → Rejected**, providing transparency in processing.  
- The workflow ensures proper checks before approval, preventing fraudulent or incorrect claim processing.

## Phase 8: Lightning Page & UI Design
- Created custom Lightning pages for Customers, Policies, Claims, and Mentors/Agents.  
- Added related lists to show linked records, improving navigation and user experience.  
- Clean UI design ensures:
  - Ease of use for agents and managers
  - Quick access to critical data
  - Enhanced visibility of linked records, helping in decision-making and faster approvals

## Phase 9: Reports & Dashboards
- Created reports for monitoring critical data:
  - **Claims by Status** to track pending, approved, and rejected claims
  - **Policies nearing Renewal** to ensure timely customer reminders
- Built dashboards to visualize key metrics:
  - Pending claims
  - Policy renewal alerts
- Reports and dashboards allow managers to monitor operations in real-time, improving responsiveness and efficiency.
