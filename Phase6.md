# Phase 6: Reports & Dashboards – User Interface Development

This phase focused on creating visual representations of key metrics in the Insurance Claim & Policy Management System. Charts and dashboards were used to help Managers and Admins monitor claims, policies, and customer activity effectively.

---

## 1️⃣ Reports with Charts

**Reports Created:**

- **Claims by Status** – Track the number of claims that are Pending, Approved, or Rejected.  
- **Policies Near Renewal** – Identify policies approaching their end date for renewal reminders.

**Procedure:**

1. Navigate to **Reports → New Report**.  
2. Select **Claims** (or **Policies**) as the report object.  
3. Apply filters:  
   - Claims: `Status = Pending / Approved / Rejected`  
   - Policies: `End Date = Next 30 Days`  
4. Group Rows:  
   - Claims: Group by `Status`  
   - Policies: Group by `Policy Type`  
5. Click **Add Chart** (top-right of report builder).  
6. Select **Chart Type**:  
   - Claims: **Bar Chart**  
   - Policies: **Donut Chart**  
7. Configure axes and labels.  
8. Click **Save & Run** to generate the report with chart.

**Purpose:** Provides quick insights to Managers on pending claims and expiring policies.

---

## 2️⃣ Dashboard

**Dashboard Created:**

- **Insurance Management Dashboard** – combines key charts to visualize operational metrics in one place.

**Components Added:**

1. **Pending Claims** – Bar Chart showing number of Pending, Approved, and Rejected claims.  
2. **Policies Near Renewal** – Donut Chart showing upcoming policy expirations.  
3. **Total Customers** – Metric component showing total active customers.

**Procedure:**

1. Navigate to **Dashboards → New Dashboard**.  
2. Name it: `Insurance Management Dashboard`.  
3. Click **+ Component → Select Report** (from created reports).  
4. Select chart type and configure display options.  
5. Arrange multiple components on the canvas for clear visualization.  
6. Save and **Refresh Dashboard** to view live data.

**Purpose:** Allows Managers and Admins to monitor operations in real-time, take decisions, and follow up on pending tasks efficiently.
