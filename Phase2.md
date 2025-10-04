Phase 2 – Org Setup & Configuration

This phase involved configuring the Salesforce Developer Org to build a secure, structured, and role-based environment for the Insurance Claim and Policy Management System.
The goal was to ensure proper user access, data visibility, and control before creating custom objects, relationships, and automation.

1. Salesforce Developer Edition Setup

The project was developed entirely in Salesforce Lightning Developer Edition, which supports:

Custom Object and Field creation

Workflow and Validation Rules

Profiles, Roles, Permission Sets

Reports and Dashboards

A single Developer Org was used for end-to-end development and testing (no sandbox required).
This environment provided full admin access to configure the data-model and security settings.

2. User Setup

Three users were created to simulate the working hierarchy:

Administrator – complete access to configure and monitor all modules

Manager – reviews and approves claims, monitors agent activities

Agent – creates and manages customers, policies, and claim records

Each user account was assigned a role and profile to reflect real-world responsibilities.
Test logins were used to verify access privileges for each type of user.

3. Profiles Configuration

Custom profiles were set up to define object-level and field-level access:

System Administrator Profile: Full CRUD access on all objects (Customers, Policies, Claims, Mentors)

Manager Profile: Read and Edit access on records created by their agents

Agent Profile: Create and View access only for their own records

Field-level security was applied to hide or make read-only sensitive data such as Claim Amount or Policy Coverage for lower roles.

Brief Purpose:
Profiles control the baseline permissions for each type of user and ensure that sensitive policy or claim data cannot be modified by unauthorized roles.

4. Role Hierarchy

A hierarchical structure was implemented as:

Admin → Manager → Agent

Agents can view and edit only their own records

Managers can view and approve the records of their reporting agents

Admin has full organization-wide visibility

Brief Purpose:
Role hierarchy establishes the approval and reporting chain, enabling upward visibility in the system for monitoring and validation.

5. Permission Sets

Created an additional “Claims Extended Access” permission set:

Temporarily granted agents edit permission on claim status during workflow testing

Allowed controlled flexibility without changing the base profile

Brief Purpose:
Permission sets were used to temporarily extend access to specific users without altering their default profile permissions.

6. Organization-Wide Defaults (OWD)

Configured base record-level security for all custom objects:

Object	Default Access	Description
Customers	Private	Only owner (agent) and their manager can view/edit
Policies	Controlled by Parent	Access inherited from related Customer
Claims	Private	Only record owner or approver can view/edit

Brief Purpose:
OWD ensures data confidentiality and prevents unauthorized data visibility between different agents.

7. Sharing Rules

Created a Manager-Level Sharing Rule to automatically share all agent-owned records with their respective managers:

Enabled Managers to review, verify, and approve claim or policy details created by agents

Brief Purpose:
Sharing rules extend record access upward in the hierarchy for supervision and claim verification.

8. Login Access & Testing

Enabled Admin login access for troubleshooting user-level issues.
Each configuration was tested by logging in as Admin, Manager, and Agent to confirm proper visibility and permission flow.

Brief Purpose:
Testing verified that security and record-sharing behaviors worked correctly before moving to customization and automation.

9. Developer Org Verification

All configurations, metadata, and role-based rules were created and tested inside a single Salesforce Developer Org.
Verified successful:

Role-based access control

Record visibility flow

Field-level security restrictions

Claim approval visibility from Agent → Manager → Admin
