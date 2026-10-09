# Travel Marketplace — Expanding Revenue Beyond Flight Bookings

**Business Analysis | Product Discovery | Marketplace Strategy | Requirements Engineering | UAT**

## Overview

This case study explores how business analysis helped shape the expansion of a travel business beyond its traditional dependence on flight bookings into a broader travel marketplace.

The proposed marketplace brought together internally managed products and external travel providers, enabling customers to discover and purchase multiple travel-related services through a shared platform.

The case study demonstrates how I approached business discovery, stakeholder alignment, marketplace governance, requirements definition, customer journeys, commercial reporting, and user acceptance testing.

> **Portfolio note:** This is a reconstructed professional case study. It excludes confidential company information, customer data, credentials, and proprietary implementation details. Recommendations and retrospective analysis are distinguished from confirmed project activities where applicable.

---

## 1. The Business Challenge

The business relied heavily on flight bookings in a competitive travel market. Customers could compare prices across providers or book directly with airlines, creating pressure to diversify the company's value proposition and revenue opportunities.

During brainstorming, I championed a discovery discussion around expanding the offering beyond flight bookings.

The opportunity was to develop a marketplace that could support products and services such as:

* Flights
* Hotels
* Tours and holiday packages
* Car hire
* Airport concierge and protocol services
* Destination activities
* Study programmes
* Other travel-related services

A key strategic question emerged: should the marketplace feature only internally managed products, or should it also accommodate external travel agencies and service providers?

Opening the marketplace to external providers could broaden product selection, while introducing a need for consistent product governance, commercial reporting, and operational accountability.

---

## 2. My Role and Contribution

As the Business Analyst, I championed a discovery session to explore how the business could expand beyond its dependence on flight bookings. I facilitated stakeholder discussions, helped translate business needs into functional requirements, and supported sprint planning and User Acceptance Testing.

My contributions included:

* **Business discovery:** Helped identify opportunities to diversify the company's travel offerings and support participation by external providers.
* **Requirements engineering:** Documented stakeholder needs, user stories, acceptance criteria, business rules, and operational workflows.
* **Marketplace governance:** Proposed a dedicated Marketplace Administrator to support consistent product reviews and fair treatment of internal and external providers.
* **Commercial rules:** Helped define optional paid product boosting while keeping standard product approval and visibility rules consistent.
* **Operational workflows:** Mapped product approval, customer checkout, inventory or capacity updates, booking notifications, fulfilment, and cancellation handling.
* **Management reporting:** Translated leadership priorities into dashboard requirements covering revenue sources, customer growth, vendor growth, destination performance, and return on investment.
* **Quality assurance:** Supported UAT to validate marketplace workflows against documented acceptance criteria.


---

## 3. The Proposed Marketplace Model

The marketplace connected five core areas:

1. **Product supply:** Internal departments and external vendors create and submit products.
2. **Governance:** A Marketplace Administrator reviews products against marketplace guidelines.
3. **Customer discovery:** Customers browse categories, search for products, and discover destination-related services.
4. **Transactions and fulfilment:** Customers purchase through the website; the responsible product owner or vendor handles fulfilment.
5. **Business intelligence:** Reporting supports product governance, vendor activity, revenue analysis, customer growth, and ROI evaluation.

### Core design principle

> **Centralise what needs consistency; decentralise what requires product ownership.**

Marketplace approval, visibility rules, and core reporting require consistent governance. Product ownership and fulfilment remain with the responsible internal department or external provider.

---

## 4. Business and Product Decisions

### Open marketplace model

The marketplace concept extended beyond internal products to accommodate external providers, broadening potential product supply.

### Neutral product governance

I proposed a dedicated Marketplace Administrator to review submitted products and approve or reject them against defined guidelines.

Internal and external products were intended to follow the same core approval process.

### Unified purchase journey

Customers could select multiple eligible travel products, add them to a cart, and proceed through the website's checkout and payment process.

### Paid product boosting

Vendors could choose to pay for increased product visibility. Boosting affected placement but did not replace the approval requirement.

### Vendor-led fulfilment

After purchase, the relevant vendor or internal product owner received the information needed to fulfil the booking.

### Commercial reporting

Management needed visibility into internal product revenue, external vendor revenue, customer growth, vendor growth, and marketplace ROI—not just product views.

---

## 5. Business Process & Customer Journey

The marketplace was considered as an end-to-end business service:

**Discover → Explore → Select → Cart → Payment → Confirmation → Fulfilment → Reporting**

This approach helped connect customer-facing functionality with vendor operations and commercial outcomes.

---

## 6. Case Study Documentation

### Business Context and Strategy

* [Business Context](docs/business-context.md)
* [Stakeholder Analysis](docs/stakeholder-analysis.md)
* [Marketplace Model](docs/marketplace-model.md)

### Requirements and Business Analysis

* [Requirements](docs/requirements.md)
* [User Stories](docs/user-stories.md)
* [Business Rules](docs/business-rules.md)
* [Requirements Traceability Matrix](artifacts/requirements-traceability-matrix.md)

### Process Diagrams

* [Customer Journey](diagrams/customer-journey.md)
* [Vendor Journey](diagrams/vendor-journey.md)
* [Marketplace Ecosystem](diagrams/marketplace-ecosystem.md)
* [Product Approval Flow](diagrams/product-approval-flow.md)

### Discovery, Testing and Reporting

* [Marketplace Search & Discovery Matrix](artifacts/marketplace-search-matrix.md)
* [UAT Test Scenarios & Results](artifacts/uat-test-scenarios.md)
* [Dashboard Requirements](artifacts/dashboard-requirements.md)

---

## 7. UAT & Requirements Traceability

The case study documents a UAT scenario set spanning:

* Customer registration and product discovery
* Vendor onboarding and product submission
* Product approval, rejection, and visibility
* Product boosting
* Cart, checkout, and online payment
* Quantity and availability management
* Vendor fulfilment
* Cancellation and voucher handling
* Marketplace administration and reporting

The Requirements Traceability Matrix links business requirements to user stories, business rules, and corresponding UAT scenarios.

**Important:** The documented scenarios demonstrate test design and traceability. Actual execution outcomes should be published only where supported by the original test records. Any reconstructed or illustrative results should be labelled accordingly.

---

## 8. Business Value & Success Measures

The marketplace was intended to support business diversification and create additional commercial opportunities.

The main measures identified for management included:

| Measure                  | Business Purpose                                                        |
| ------------------------ | ----------------------------------------------------------------------- |
| Internal product revenue | Understand revenue generated from company-owned products                |
| External vendor revenue  | Understand the commercial contribution of external providers            |
| Customer growth          | Assess whether marketplace activity contributes to customer acquisition |
| Vendor growth            | Monitor marketplace supply-side expansion                               |
| New vendor registrations | Track provider onboarding                                               |
| Marketplace sales        | Monitor transaction activity                                            |
| ROI                      | Evaluate commercial value relative to marketplace investment            |

These are intended measures of business performance, not claims of quantified outcomes. No unverified revenue, conversion, or growth figures are asserted in this case study.

---

## 9. Key Business Analysis Lessons

### Strategy must translate into operating processes

Expanding into a marketplace creates new questions around governance, vendor participation, transactions, fulfilment, and accountability.

### Neutral governance supports scale

A consistent approval process helps maintain marketplace standards across products from different owners.

### Customer journeys should connect to business outcomes

Search, discovery, checkout, and fulfilment need to work together to support completed purchases and customer satisfaction.

### Reporting should support decisions

Operational activity metrics are useful, but executive reporting must connect activity to revenue, growth, and return on investment.

### UAT must validate the whole business journey

A successful marketplace depends on more than individual features. The customer transaction, vendor fulfilment, and management reporting processes must work together.

---

## 10. Skills Demonstrated

* Business discovery and problem definition
* Stakeholder engagement and facilitation
* Product and marketplace strategy
* Business requirements documentation
* User stories and business rules
* Process modelling
* Requirements traceability
* Customer journey analysis
* UAT planning and coordination
* Commercial KPI and dashboard requirements
* Vendor governance and operational workflow analysis
* Cross-functional collaboration

---

## Conclusion

This case study demonstrates my approach to translating a business diversification opportunity into a structured marketplace concept, supported by defined actors, governance processes, requirements, customer journeys, testing scenarios, and commercial reporting needs.

It reflects a business analysis mindset focused not only on documenting features, but also on understanding **why the business needs a solution, how the solution should operate, and how its value should be evaluated**.
