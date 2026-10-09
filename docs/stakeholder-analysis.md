# Stakeholder Analysis — Travel Marketplace

## 1. Purpose

This document identifies the main stakeholders involved in the travel marketplace, their interests, responsibilities, expectations, and influence on the solution.

The stakeholder analysis supported requirements gathering, clarification of operational responsibilities, and alignment around a marketplace model that could accommodate both internal product owners and external providers.

## 2. Stakeholder Overview

| Stakeholder                    | Primary Interest                                    | Main Responsibilities                                                              | Key Information Needs                                                               |
| ------------------------------ | --------------------------------------------------- | ---------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------- |
| Executive Management           | Commercial growth and business performance          | Set strategic direction and evaluate marketplace performance                       | Revenue, customer growth, vendor growth, and ROI                                    |
| Marketplace Administrator      | Product quality and marketplace governance          | Review submissions, approve or reject products, and oversee marketplace operations | Product status, submission details, rejection reasons, and sales information        |
| Internal Product Owners        | Sell and manage company-owned products              | Create products, submit them for approval, and fulfil bookings                     | Product status, purchases, customer details, and revenue                            |
| External Vendors               | Reach customers and generate sales                  | Register, submit products, manage bookings, and fulfil services                    | Approval feedback, purchases, customer information, and earnings                    |
| Customers / Travellers         | Discover and purchase relevant travel services      | Search, review, select, and purchase products                                      | Product information, availability, pricing, and purchase confirmation               |
| Finance Team                   | Financial visibility and transaction accountability | Support financial monitoring and vendor-related reporting                          | Transaction records, revenue information, and vendor statements                     |
| Operational / Fulfilment Teams | Deliver purchased services                          | Coordinate bookings and fulfilment where responsible                               | Traveller information, product details, booking status, and fulfilment requirements |
| Development / QA Team          | Deliver and validate the solution                   | Implement requirements, investigate defects, and support testing                   | Business rules, user stories, acceptance criteria, and test scenarios               |

## 3. Stakeholder Analysis

### 3.1 Executive Management

**Interest:** High
**Influence:** High

Executive management needed to understand whether the marketplace could contribute to the wider business beyond the introduction of new website features.

The main reporting priorities included:

* Revenue from internal products.
* Revenue from external vendors.
* Customer growth.
* Customers directed to the main BTM Holidays website.
* Vendor growth and new vendor registrations.
* Marketplace performance and ROI.

**Business Analyst approach:** Translate strategic objectives into measurable reporting requirements and ensure that dashboard discussions focused on business outcomes rather than activity metrics alone.

### 3.2 Marketplace Administrator

**Interest:** High
**Influence:** High

The Marketplace Administrator was proposed as a central governance role responsible for reviewing product submissions and controlling marketplace approval.

Responsibilities included:

* Reviewing products against marketplace guidelines.
* Approving compliant products.
* Rejecting non-compliant products with feedback.
* Monitoring product status and marketplace activity.
* Supporting consistent treatment of internal and external products.

**Business Analyst approach:** Define the approval workflow, clarify decision ownership, and establish the relationship between product approval and customer visibility.

### 3.3 Internal Product Owners

**Interest:** High
**Influence:** Medium to High

Internal departments could act as product owners within the marketplace.

They needed to create and manage products, receive relevant purchase information, fulfil bookings, and understand their commercial contribution.

A key design consideration was ensuring that internal products followed the same core approval process as external products.

**Business Analyst approach:** Capture internal product-owner needs while maintaining neutral marketplace governance.

### 3.4 External Vendors

**Interest:** High
**Influence:** Medium

External vendors needed a clear way to participate in the marketplace and sell products to customers.

Their principal needs included:

* Vendor registration and onboarding.
* Product creation and submission.
* Approval or rejection feedback.
* Product visibility.
* Purchase notifications.
* Access to relevant customer information for fulfilment.
* Visibility into sales and earnings.

**Business Analyst approach:** Consider the vendor journey from onboarding through product approval, purchase notification, fulfilment, and reporting.

### 3.5 Customers / Travellers

**Interest:** High
**Influence:** Medium

Customers needed a straightforward way to discover relevant travel services and complete purchases.

Key customer needs included:

* Clear product categories.
* Search and browsing.
* Relevant destination-related discovery.
* Product details and availability.
* A cart supporting multiple eligible products.
* Website-based checkout and payment.
* Purchase confirmation.
* Clear handling of applicable cancellations and vouchers.

**Business Analyst approach:** Map the end-to-end customer journey and consider how each stage connects to the next.

### 3.6 Finance Team

**Interest:** High
**Influence:** Medium to High

Finance-related reporting needed to support visibility into marketplace transactions and vendor-level financial information.

Relevant requirements included transaction records, revenue reporting, and vendor statements of account.

**Business Analyst approach:** Identify the information required for financial monitoring and reporting without assuming unconfirmed accounting or settlement automation.

### 3.7 Operational and Fulfilment Teams

**Interest:** High
**Influence:** Medium

The responsible vendor or internal product owner needed the information required to fulfil a purchased service.

This could include customer contact details, product purchased, quantity, booking date, participant information, payment status, and fulfilment status.

**Business Analyst approach:** Clarify the handover from purchase confirmation to fulfilment and establish what information each responsible party needs.

### 3.8 Development and QA Team

**Interest:** High
**Influence:** Medium to High

The development and QA teams needed requirements that could be understood, implemented, and validated.

Their needs included:

* Clear business requirements.
* Defined business rules.
* User stories and acceptance criteria.
* Process diagrams.
* Traceability between requirements and tests.
* Testable expected outcomes.

**Business Analyst approach:** Structure requirements so that business intent could be traced into implementation and UAT.

## 4. Stakeholder Interests and Potential Tensions

Several areas required stakeholder alignment.

| Topic                             | Potential Tension                                    | Business Analysis Response                                                                   |
| --------------------------------- | ---------------------------------------------------- | -------------------------------------------------------------------------------------------- |
| Marketplace participation         | Internal-only versus open marketplace                | Facilitate discussion of product breadth, growth opportunities, and operational implications |
| Product approval                  | Product owners want their products published quickly | Define a consistent review and approval process                                              |
| Internal versus external products | Risk of perceived preferential treatment             | Propose neutral governance under the Marketplace Administrator                               |
| Visibility and boosting           | Organic discovery versus paid placement              | Distinguish approval requirements from optional paid visibility                              |
| Reporting                         | Activity metrics versus commercial outcomes          | Prioritise management's revenue, growth, and ROI questions                                   |
| Fulfilment                        | Marketplace transaction versus service delivery      | Clarify vendor/product-owner responsibility after purchase                                   |

These tensions illustrate why stakeholder engagement was important before finalising requirements.

## 5. Stakeholder Engagement Approach

The Business Analyst approach involved:

1. Identifying stakeholder groups and their objectives.
2. Facilitating discovery and requirements discussions.
3. Clarifying disagreements and competing priorities.
4. Translating decisions into business rules and workflows.
5. Documenting requirements and user stories.
6. Supporting sprint planning and delivery discussions.
7. Coordinating UAT around agreed business processes.
8. Connecting reporting needs to management decisions.

## 6. Key Stakeholder Decisions

The marketplace design incorporated the following principles:

* Internal and external products follow the same core approval process.
* A dedicated Marketplace Administrator provides central product governance.
* Vendors and internal product owners remain responsible for their products and fulfilment.
* Customers use a shared marketplace discovery and purchase journey.
* Paid boosting can increase visibility but cannot bypass approval.
* Management reporting distinguishes internal and external revenue.
* Commercial performance is evaluated using business-oriented measures, not product views alone.

## 7. Business Analyst Contribution

My contribution was to help bridge differences between strategic expectations, operational requirements, vendor needs, customer experience, and reporting priorities.

Rather than treating stakeholder requests as isolated features, I considered how the decisions affected the marketplace operating model as a whole.

## 8. Key Takeaway

Effective stakeholder analysis requires understanding not only who the stakeholders are, but also what decisions they need to make, what outcomes they value, and where their priorities may conflict.

**Core principle:** Align stakeholder expectations before translating them into requirements, business rules, and testable outcomes.
