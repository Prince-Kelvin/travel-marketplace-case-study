# Marketplace Operating Model

## 1. Purpose

This document describes the proposed operating model for the travel marketplace, including product supply, governance, customer transactions, vendor fulfilment, and commercial reporting.

The model was intended to support products from both internal departments and external providers while maintaining consistent marketplace governance.

## 2. Marketplace Concept

The marketplace extends the traditional travel-booking model beyond flight bookings.

It brings multiple travel-related products into a shared digital environment where customers can discover and purchase services from different product owners.

Potential product categories include:

* Flights
* Hotels
* Tours and holiday packages
* Car hire
* Airport concierge and protocol services
* Destination activities
* Study programmes
* Other travel-related services

The marketplace serves as the shared platform, while the responsible product owner or vendor remains accountable for delivering the purchased service.

## 3. Operating Model Overview

The operating model consists of six connected stages:

1. Product supply
2. Product submission
3. Marketplace governance
4. Customer discovery and transaction
5. Vendor fulfilment
6. Commercial reporting

### High-Level Process

```text
Internal Product Owners     External Vendors
           |                       |
           +-----------+-----------+
                       |
                Product Creation
                       |
                Product Submission
                       |
             Marketplace Administrator
                       |
                Review and Decision
                  /           \
              Approve        Reject
                 |              |
                 |         Feedback / Revision
                 |              |
                 |          Resubmission
                 |
          Customer Visibility
                 |
        Search / Browse / Discover
                 |
            Product Details
                 |
                 Cart
                 |
          Website Checkout
                 |
             Payment
                 |
        Purchase Confirmation
                 |
       Vendor / Product Owner
                 |
             Fulfilment
                 |
         Marketplace Reporting
                 |
        Executive Business Review
```

## 4. Product Supply Model

### 4.1 Internal Product Owners

Internal departments can create and manage products within their areas of responsibility.

Examples may include company-managed travel packages, concierge services, or other internally managed offerings.

Internal product owners submit products through the marketplace's approval process and remain responsible for fulfilment where applicable.

### 4.2 External Vendors

External travel agencies and service providers can register and submit products for consideration.

The open marketplace model expands potential product supply beyond services managed directly by the company.

External vendors are subject to the same core product governance process as internal product owners.

### 4.3 Shared Product Governance

The marketplace is not intended to operate two separate approval systems for internal and external products.

Instead, both groups use a common process for product submission, review, approval, and customer visibility.

**Operating principle:** One marketplace process, regardless of who owns the product.

## 5. Marketplace Governance

A dedicated Marketplace Administrator was proposed to provide a neutral point of control over product approval.

The administrator's responsibilities include:

* Reviewing submitted products against marketplace guidelines.
* Approving compliant products.
* Rejecting products that do not meet requirements.
* Providing rejection feedback.
* Managing the transition from submission to customer visibility.
* Supporting consistent marketplace standards.

A product should not become customer-visible before approval.

This governance model supports quality control and reduces the risk of internal products receiving preferential treatment.

## 6. Customer Discovery Model

Customers can discover products through marketplace categories, search, browsing, and destination-related recommendations.

The marketplace should support both direct and complementary discovery.

For example, a customer planning a trip may initially be interested in a flight but could also discover accommodation, tours, activities, or concierge services associated with the destination.

This creates opportunities for cross-selling relevant products within the same customer journey.

The exact search fields, filter behaviour, and recommendation logic depend on the implemented functionality and should not be assumed without supporting requirements.

## 7. Paid Product Boosting

The marketplace includes an optional paid visibility concept.

During product creation, a vendor can indicate whether they want to boost a product. An eligible approved product may also be boosted later.

A boost provides increased visibility by placing the product higher in marketplace results.

### Key Principles

* Boosting is optional.
* The applicable fee is additional to the product's normal commercial terms.
* A product must still pass the marketplace approval process.
* Boosting does not replace product governance.
* Internal and external products should be governed consistently.

Product views may provide useful activity information, but management's principal reporting interest is in revenue, customer growth, vendor growth, and ROI.

## 8. Customer Transaction Model

The intended customer journey is:

**Discover → Select → Cart → Checkout → Payment → Confirmation**

Customers can select multiple eligible products and add them to a shared cart.

For example, a customer may select a flight, hotel, tour, and concierge service within one purchase journey.

The checkout and payment process takes place through the marketplace website rather than requiring customers to complete separate payments across unrelated channels.

Following a successful purchase, the customer receives a purchase confirmation.

## 9. Product Quantity and Availability

Approved products may have defined quantities, capacities, or participant limits.

For example, a group tour may have a minimum participant requirement and a booking deadline.

The marketplace should reflect purchased quantities appropriately and provide visibility into applicable availability.

Where a product depends on a minimum participant threshold, the vendor determines whether to proceed if the threshold is not reached by the relevant deadline.

If the vendor decides not to proceed, the applicable cancellation process is initiated in accordance with the marketplace terms.

## 10. Vendor Fulfilment Model

After purchase, the responsible vendor or internal product owner receives a notification and the information required to fulfil the booking.

Relevant information may include:

* Customer name and contact information
* Product purchased
* Quantity
* Booking date
* Participant or traveller details
* Payment status
* Fulfilment status

The vendor or internal product owner handles the product-specific fulfilment process.

This separates the shared marketplace transaction from the operational delivery of each service.

## 11. Cancellation and Voucher Handling

Some products may have conditions such as minimum participant requirements or booking deadlines.

Where a vendor decides not to proceed with a product, the relevant cancellation process follows the applicable terms and conditions.

For the described group-tour scenario:

1. The booking deadline is reached.
2. The minimum participant requirement has not been met.
3. The vendor decides not to proceed.
4. The vendor notifies the platform.
5. Eligible bookings are cancelled under the applicable terms.
6. The customer receives a voucher equivalent to the refunded amount, according to the agreed process.

The voucher allows the customer to spend the corresponding value on another eligible product.

## 12. Reporting and Business Intelligence

The marketplace requires different reporting views for operational users and management.

### 12.1 Marketplace Administrator

Key reporting needs include:

* Total products uploaded
* Pending approvals
* Declined products
* Total sales
* Gross revenue
* Sales by vendor
* Sales by destination
* Top destination
* Top vendor
* Vendor statements of account

### 12.2 Vendor / Internal Product Owner

Relevant performance information includes:

* Product views
* Purchases
* Revenue earned
* Boosting expenditure

Conversion rate was identified as a possible later enhancement rather than a mandatory initial requirement.

### 12.3 Executive Management

Management's priorities include:

* Revenue from internal products
* Revenue from external vendors
* Customer growth
* Customers directed to the main BTM Holidays website
* Vendor growth
* New vendor registrations
* Marketplace performance
* ROI

These reporting requirements are intended to help management evaluate the marketplace's commercial contribution to the wider business.

## 13. Business Model Principles

The marketplace operating model is guided by the following principles.

### Centralise what needs consistency

Central governance supports product approval, visibility rules, the shared customer transaction experience, and core reporting.

### Decentralise what requires product ownership

Vendors and internal departments retain responsibility for their products and fulfilment activities.

### Connect customer experience to commercial value

Product discovery, checkout, fulfilment, and reporting should work together to support a coherent business service.

### Measure outcomes, not activity alone

Views and other activity metrics can be useful, but revenue, customer growth, vendor growth, and ROI are more directly aligned with management's strategic questions.

## 14. Business Analyst Contribution

My Business Analyst contribution included helping shape the marketplace concept, facilitating stakeholder discussions, proposing a dedicated Marketplace Administrator, coordinating requirements gathering and sprint planning, and supporting UAT.

The analysis considered the relationship between the commercial model, product governance, customer journeys, fulfilment responsibilities, and management reporting.

## 15. Key Takeaway

The marketplace model combines a shared digital transaction environment with distributed product ownership and fulfilment.

Its success depends on aligning:

**Product Supply → Governance → Customer Discovery → Transaction → Fulfilment → Business Intelligence**

This provides a structured foundation for expanding product choice while maintaining consistent governance and supporting evaluation of commercial performance.
