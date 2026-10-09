# Stakeholder & Persona Analysis

## 1. Purpose

The marketplace involved multiple stakeholder groups with different objectives, responsibilities and expectations.

The stakeholder analysis was therefore important for understanding:

* Who interacts with the marketplace.
* Who owns products.
* Who approves products.
* Who fulfils purchases.
* Who consumes marketplace services.
* Who monitors performance.
* Who makes strategic decisions.

A key design principle was to avoid creating separate marketplace processes for internal and external product owners where the underlying business activity was the same.

---

# 2. Stakeholder Overview

| Stakeholder               | Primary Interest                           | Key Responsibility                                     |
| ------------------------- | ------------------------------------------ | ------------------------------------------------------ |
| Traveller                 | Discovering and purchasing travel products | Search, select, purchase and consume services          |
| External Vendor           | Selling travel products                    | Product creation, fulfilment and customer servicing    |
| Internal Product Owner    | Selling company-owned products             | Product ownership and fulfilment                       |
| Marketplace Administrator | Marketplace governance                     | Product review, approval and operational monitoring    |
| Executive Management      | Commercial performance                     | Strategy, investment and ROI                           |
| Fulfilment Team           | Delivering purchased services              | Service fulfilment and customer support                |
| Business Analyst          | Business and product alignment             | Discovery, requirements, process analysis and UAT      |
| Technology/Delivery Team  | Platform delivery                          | Development, configuration, integration and deployment |

---

# 3. Traveller Persona

### Persona

**Primary marketplace customer**

### Objective

Find and purchase travel products through a convenient and unified digital experience.

### Typical Needs

* Search for travel products.
* Browse products by category or destination.
* View product information.
* Add products to a cart.
* Purchase multiple products.
* Complete payment through one platform.
* Receive purchase confirmation.
* Access the service purchased.

### Pain Points

A traveller planning a trip may need multiple services, including:

* Flights
* Hotels
* Tours
* Activities
* Airport concierge
* Car hire
* Holiday packages

Having to purchase each service through separate platforms could create additional effort and fragmented payment experiences.

### Marketplace Value

The marketplace provides a central point for discovering and purchasing multiple travel services.

---

# 4. External Vendor Persona

### Persona

**Travel agency or travel service provider**

### Objective

Use the marketplace as an additional channel for reaching customers and generating sales.

### Typical Needs

* Register as a marketplace vendor.
* Create products.
* Upload product information and images.
* Submit products for approval.
* Monitor product performance.
* Receive purchase notifications.
* Access customer/order information.
* Fulfil purchases.
* Monitor revenue.
* Purchase additional product visibility where required.
* Generate or access financial information relating to marketplace sales.

### Pain Points

External providers need sufficient visibility and commercial value to justify participating in the marketplace.

A marketplace with many vendors but limited customer demand would provide limited value to them.

### Marketplace Value

The marketplace provides:

* Product distribution.
* Customer access.
* Transaction processing.
* Product visibility.
* Performance information.
* Additional sales opportunities.

---

# 5. Internal Product Owner Persona

### Persona

**Company department responsible for a marketplace product**

Internal departments could curate and own products in the same marketplace environment as external vendors.

Examples include teams responsible for:

* Tour packages.
* Hotel deals.
* Airport concierge services.
* Other travel products.

### Objective

Create, manage and fulfil products offered through the marketplace.

### Key Responsibilities

* Create products.
* Provide product information.
* Upload product images.
* Submit products for approval.
* Monitor purchases.
* Receive customer information.
* Manage fulfilment.
* Manage product availability where applicable.

### Design Principle

Internal departments were intentionally treated as marketplace vendors for their respective products.

This avoided creating a separate preferential workflow simply because the product originated from within the company.

---

# 6. Marketplace Administrator Persona

### Persona

**Dedicated marketplace governance and operations role**

The Marketplace Administrator was responsible for maintaining marketplace standards and monitoring marketplace activity.

### Objective

Ensure that products published on the marketplace comply with approved guidelines and that marketplace operations remain visible and controlled.

### Key Responsibilities

* Review submitted products.
* Validate products against approved guidelines.
* Approve compliant products.
* Decline products that do not meet requirements.
* Provide feedback for declined products.
* Monitor marketplace products.
* Monitor sales.
* Monitor vendor performance.
* Monitor destination performance.
* Generate vendor statements of account.
* Monitor overall marketplace activity.

### Key Dashboard Information

* Total products.
* Pending approvals.
* Declined products.
* Total sales.
* Sales by vendor.
* Sales by destination.
* Top vendors.
* Top destinations.
* Gross revenue.
* Vendor statements.

### Decision Rights

The Marketplace Administrator controls whether a submitted product is approved for publication.

---

# 7. Executive Management Persona

### Persona

**Business leadership / investment stakeholders**

### Objective

Determine whether the marketplace is delivering sufficient commercial value relative to the investment made in the platform.

### Key Information Required

#### Revenue

* Internal product revenue.
* External vendor revenue.
* Overall marketplace revenue.

#### Customer Growth

* Customer growth.
* Customers directed to the main BTM Holidays website.

#### Vendor Growth

* Total vendors.
* New vendor registrations.
* Vendor growth over time.

#### Strategic Performance

* Marketplace performance.
* Return on investment.

### Decision Need

Executives do not necessarily require the same operational detail as the Marketplace Administrator.

Their primary question is:

> **Is the marketplace creating sufficient business value to justify continued investment?**

---

# 8. Fulfilment Persona

### Persona

**Team or vendor responsible for delivering the purchased travel service**

### Objective

Successfully deliver the product purchased by the traveller.

### Information Required

The fulfilment owner needs access to information such as:

* Customer name.
* Customer contact details.
* Product purchased.
* Quantity.
* Payment status.
* Booking date.
* Number of participants.
* Traveller details.
* Fulfilment status.

### Responsibility

Once a transaction is completed, the relevant vendor or internal product owner takes responsibility for fulfilment.

The marketplace facilitates the transaction and provides the information necessary for the fulfilment process.

---

# 9. Business Analyst Persona

### Persona

**Business Analysis / Product Discovery**

### Objective

Ensure that the marketplace solves the intended business problem while translating stakeholder needs into clear, testable and implementable requirements.

### Key Responsibilities

* Champion discovery discussions.
* Facilitate stakeholder conversations.
* Challenge assumptions.
* Analyse business needs.
* Define requirements.
* Identify business rules.
* Analyse customer and vendor journeys.
* Coordinate requirements.
* Support sprint planning.
* Coordinate UAT.
* Validate that delivered functionality supports business objectives.

### BA Perspective

The Business Analyst role extended beyond documenting stakeholder requests.

The analysis considered:

**Business Strategy → Stakeholders → Customer Experience → Vendor Experience → Operational Process → Technology Requirements → Validation**

---

# 10. Stakeholder Influence & Interest

A simplified stakeholder model was used to consider stakeholder involvement.

| Stakeholder               | Influence | Interest | Engagement Approach                       |
| ------------------------- | --------- | -------- | ----------------------------------------- |
| Executive Management      | High      | High     | Strategic reporting and decision-making   |
| Marketplace Administrator | High      | High     | Continuous operational engagement         |
| External Vendors          | Medium    | High     | Requirements, onboarding and feedback     |
| Internal Product Owners   | Medium    | High     | Product and fulfilment requirements       |
| Travellers                | High      | High     | Customer journey and usability validation |
| Fulfilment Teams          | Medium    | High     | Workflow and operational validation       |
| Technology/Delivery Team  | High      | High     | Requirements clarification and delivery   |
| Business Analyst          | High      | High     | Cross-functional coordination             |

---

# 11. Key Stakeholder Conflicts & Resolution

Several stakeholder questions required business analysis rather than simply capturing individual preferences.

### Conflict 1 — Internal vs External Marketplace

**Question:** Should the marketplace only promote company-owned products?

**Analysis:** Limiting supply could restrict product variety and marketplace growth.

**Decision:** Open the marketplace to external providers.

---

### Conflict 2 — Product Preference

**Question:** Should certain products receive preferential organic placement?

**Analysis:** Informal preferential treatment could undermine marketplace neutrality and create vendor concerns.

**Decision:** Approved products receive equal organic treatment.

**Commercial alternative:** Vendors can pay for explicit product boosting.

---

### Conflict 3 — Central Control vs Product Ownership

**Question:** Should each department manage its own publication process?

**Analysis:** Multiple approval approaches could result in inconsistent marketplace standards.

**Decision:** Centralise product approval through the Marketplace Administrator while retaining product ownership and fulfilment responsibility with the relevant team/vendor.

---

### Conflict 4 — Marketplace Convenience vs Vendor Ownership

**Question:** Should the platform manage the entire service fulfilment process?

**Analysis:** Vendors and internal product teams have the operational knowledge required to deliver their respective products.

**Decision:** The marketplace manages discovery, transaction and payment while the relevant vendor/product owner manages fulfilment.

---

# 12. Stakeholder Design Principle

A recurring principle throughout the marketplace design was:

> **Centralise what needs consistency; decentralise what requires product ownership.**

### Centralised

* Marketplace governance.
* Product approval.
* Marketplace transaction.
* Payment.
* Core marketplace reporting.

### Decentralised

* Product ownership.
* Product fulfilment.
* Vendor/customer servicing.
* Product-specific operational decisions.

This structure allowed the marketplace to maintain consistent governance while supporting multiple internal departments and external providers.

---

# 13. Stakeholder Success Criteria

Each stakeholder group ultimately defined marketplace success differently.

| Stakeholder               | Success Indicator                                                   |
| ------------------------- | ------------------------------------------------------------------- |
| Traveller                 | Convenient discovery and successful purchase                        |
| External Vendor           | Product sales and revenue                                           |
| Internal Product Owner    | Product sales and successful fulfilment                             |
| Marketplace Administrator | Controlled, healthy marketplace operations                          |
| Executive Management      | Revenue growth, customer growth, vendor growth and ROI              |
| Fulfilment Team           | Successful service delivery                                         |
| Business Analyst          | Business requirements successfully translated into a usable product |
| Technology/Delivery Team  | Stable implementation of agreed requirements                        |

The marketplace therefore required a balanced approach to stakeholder value rather than optimising for a single user group.
