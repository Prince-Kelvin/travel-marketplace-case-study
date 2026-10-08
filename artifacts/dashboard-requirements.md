# Dashboard Requirements

## Purpose

The marketplace required different levels of reporting for different users.

The reporting approach was designed around the decisions each stakeholder needed to make rather than presenting every user with the same information.

Three primary dashboard perspectives were identified:

1. **Marketplace Administration**
2. **Vendor / Product Owner**
3. **Executive Management**

---

# 1. Dashboard Structure

| Dashboard                   | Primary User                             | Main Purpose                                                                  |
| --------------------------- | ---------------------------------------- | ----------------------------------------------------------------------------- |
| Marketplace Admin Dashboard | Marketplace Administrator                | Manage products, approvals, vendors, transactions, and marketplace operations |
| Vendor Dashboard            | External Vendor / Internal Product Owner | Monitor products, purchases, revenue, and marketplace performance             |
| Executive Dashboard         | Management                               | Monitor commercial performance, growth, revenue contribution, and ROI         |

---

# 2. Marketplace Administrator Dashboard

## Objective

Provide the Marketplace Administrator with a central operational view of marketplace activity.

The dashboard should support product governance, transaction monitoring, vendor management, and operational reporting.

### Key Metrics

| Metric                      | Purpose                                              |
| --------------------------- | ---------------------------------------------------- |
| Total Products Uploaded     | Monitor marketplace catalogue growth                 |
| Pending Products            | Identify products awaiting approval                  |
| Declined Products           | Monitor rejected submissions and governance activity |
| Total Sales                 | Monitor marketplace transaction activity             |
| Gross Revenue               | Monitor overall marketplace revenue                  |
| Sales by Vendor             | Compare vendor-generated sales                       |
| Sales by Destination        | Identify high-performing destinations                |
| Top Destination             | Identify strongest destination performance           |
| Top Vendor                  | Identify strongest vendor performance                |
| Vendor Statement of Account | Support vendor-level transaction reporting           |

---

## Administrator Reporting Views

### Product Management

The administrator should be able to monitor:

* Products submitted
* Products pending approval
* Approved products
* Declined products
* Product status
* Product ownership/vendor

This supports the central marketplace governance model.

### Sales Reporting

Sales should be viewable across relevant business dimensions, including:

* Vendor
* Destination
* Product
* Transaction activity

This allows the administrator to identify where marketplace activity is coming from.

### Vendor Statement

The reporting layer should support generation or review of vendor-level transaction information required for statements of account.

This provides a consistent basis for reviewing vendor transactions and marketplace earnings.

---

# 3. Vendor Dashboard

## Objective

Give vendors and internal product owners visibility into the performance of their marketplace products.

### Key Metrics

| Metric               | Purpose                                           |
| -------------------- | ------------------------------------------------- |
| Product Views        | Understand customer interest                      |
| Purchases            | Monitor product sales                             |
| Total Revenue Earned | Understand commercial performance                 |
| Boosting Spend       | Track money spent on increased product visibility |
| Conversion Rate      | Evaluate movement from interest to purchase       |

### Phase 2 Enhancement

Conversion rate was identified as a useful performance metric but positioned as a later enhancement rather than a mandatory initial dashboard requirement.

This demonstrates prioritisation between **business value and implementation scope**.

---

# 4. Executive Management Dashboard

## Objective

Provide management with a high-level view of whether the marketplace is contributing to the wider business.

The executive dashboard should focus on **commercial outcomes rather than activity metrics alone**.

### Primary Management Metrics

| Metric                             | Management Question                                                                         |
| ---------------------------------- | ------------------------------------------------------------------------------------------- |
| Internal Product Revenue           | How much revenue is being generated from products uploaded by the company's internal teams? |
| External Vendor Revenue            | How much revenue is being generated from external marketplace vendors?                      |
| Customer Growth                    | Is the marketplace helping grow the customer base?                                          |
| Customers Directed to Main Website | Is marketplace activity contributing traffic/customer growth to the main travel business?   |
| Vendor Growth                      | Is the external marketplace ecosystem expanding?                                            |
| New Vendor Registrations           | Are new suppliers/providers joining the marketplace?                                        |
| Marketplace Revenue                | How much commercial value is the marketplace generating?                                    |
| ROI                                | Is the marketplace producing sufficient business value relative to investment?              |

---

# 5. Internal vs External Revenue

One of the key management requirements was the ability to distinguish between:

**Internal Product Revenue**

Revenue generated from products uploaded and managed by the company's internal departments.

versus

**External Vendor Revenue**

Revenue generated from products provided by external marketplace vendors.

This distinction allows management to understand the marketplace's contribution from two different commercial sources.

### Business Question

> Is marketplace growth being driven primarily by the company's own products, external vendors, or a combination of both?

This is more useful for strategic decision-making than looking only at total marketplace revenue.

---

# 6. Customer Growth

Customer growth was treated as an important marketplace performance indicator.

The dashboard should help management understand whether marketplace activity is contributing to growth in customers directed toward the company's main travel website.

The intended relationship is:

**Marketplace Discovery → Customer Engagement → Main Website → Customer Growth**

This connects marketplace activity to the broader business rather than treating the marketplace as an isolated platform.

---

# 7. Vendor Growth

Vendor growth provides an indication of the health of the marketplace ecosystem.

Relevant indicators include:

* Total vendors
* New vendor registrations
* Vendor activity
* Vendor-generated sales
* Vendor contribution to marketplace revenue

The objective is not simply to maximise vendor numbers.

A healthy marketplace should attract vendors who contribute useful products and meaningful commercial activity.

---

# 8. ROI

ROI was identified as a key executive-level measure.

Management's focus was primarily on whether the marketplace was generating meaningful business value rather than simply measuring feature usage.

A simplified business view is:

**Marketplace ROI = Business Value Generated ÷ Marketplace Investment**

The dashboard therefore prioritises commercial indicators such as:

* Revenue
* Customer growth
* Vendor growth
* Marketplace activity
* Investment in marketplace operations

---

# 9. Product Views vs Business Outcomes

Product views were available as a useful marketplace activity metric.

However, management's primary interest was not simply:

> "How many people viewed this product?"

The more important questions were:

> "Did the marketplace generate revenue?"

> "Did we grow our customer base?"

> "Did we attract valuable vendors?"

> "Is the marketplace producing a positive return?"

This distinction influenced the prioritisation of dashboard metrics.

### BA Insight

Not every measurable event should automatically become a primary KPI.

A useful KPI should connect activity to a meaningful **business decision or outcome**.

---

# 10. KPI Hierarchy

The dashboard requirements can therefore be viewed as a hierarchy:

### Level 1 — Activity

* Product views
* Products uploaded
* Products approved
* Vendor registrations

↓

### Level 2 — Commercial Activity

* Purchases
* Sales
* Revenue
* Vendor revenue

↓

### Level 3 — Business Outcomes

* Customer growth
* Vendor ecosystem growth
* Internal vs external revenue contribution
* ROI

This hierarchy prevents the dashboard from becoming a collection of disconnected numbers.

---

# 11. Dashboard Traceability

| Business Objective                   | Dashboard Requirement                 | Primary User       |
| ------------------------------------ | ------------------------------------- | ------------------ |
| Govern marketplace products          | Product and approval metrics          | Marketplace Admin  |
| Monitor marketplace sales            | Sales and revenue reporting           | Admin / Management |
| Understand vendor performance        | Vendor sales and revenue              | Admin / Vendor     |
| Monitor internal vs external revenue | Revenue segmentation                  | Management         |
| Grow customer base                   | Customer growth indicators            | Management         |
| Grow vendor ecosystem                | Vendor registration/growth indicators | Management         |
| Measure marketplace success          | ROI and commercial KPIs               | Management         |
| Support vendor transparency          | Vendor statement of account           | Admin / Vendor     |

---

# 12. BA Design Principle

The dashboard requirements followed a simple principle:

> **Different users need different information because they make different decisions.**

The Marketplace Administrator needs to **operate and govern** the marketplace.

The Vendor needs to **manage and improve product performance**.

Management needs to **evaluate commercial performance and strategic value**.

Therefore, the dashboard should not be treated as one generic reporting page.

---

## Key Takeaway

The marketplace reporting model moved beyond basic operational reporting toward **decision-oriented business intelligence**.

The most important question was not simply whether users were interacting with the marketplace.

It was whether the marketplace was contributing measurable value to the wider business through:

**Revenue → Customer Growth → Vendor Growth → ROI**

This helped position the marketplace as a **commercial growth channel**, rather than simply another website feature.
