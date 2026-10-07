# Marketplace Requirements

## Purpose

The marketplace requirements translated the business strategy and product discovery discussions into functional requirements that could guide design, development, sprint planning, and User Acceptance Testing (UAT).

The requirements covered the major marketplace capabilities across:

* Customer experience
* Vendor onboarding
* Product management
* Product governance
* Search and discovery
* Cart and checkout
* Payments
* Notifications
* Fulfilment
* Reporting
* Marketplace administration

---

# 1. Customer Requirements

## CR-01 — Customer Registration

The marketplace shall allow customers to create an account using supported registration methods.

Supported registration options included:

* Google
* Facebook
* Email
* Phone number

### Acceptance Criteria

* Customer can select a supported registration method.
* Successful registration creates a customer account.
* Customer can subsequently authenticate using the registered account.
* Registration errors are communicated to the customer.

---

## CR-02 — Customer Login

The marketplace shall allow registered customers to log in and access their account.

### Acceptance Criteria

* Valid credentials allow successful authentication.
* Invalid credentials are rejected.
* Appropriate feedback is displayed when authentication fails.

---

# 2. Product Discovery Requirements

## CR-03 — Product Categories

The marketplace shall organise products into relevant travel categories.

Examples include:

* Flights
* Tours
* Hotels
* Holiday packages
* Airport concierge / protocol
* Car hire
* Activities
* Study programmes
* Other travel-related products

### Acceptance Criteria

* Customer can access available product categories.
* Products are associated with the appropriate category.
* Selecting a category displays relevant products.

---

## CR-04 — Product Search

The marketplace shall allow customers to search for relevant products.

Search and discovery should support customer intent around destinations and product types.

### Acceptance Criteria

* Customer can search for available products.
* Relevant products are returned based on the search.
* Search results can be browsed.
* Appropriate feedback is provided where no relevant result exists.

---

## CR-05 — Product Pagination

The marketplace shall support pagination when displaying product results.

### Acceptance Criteria

* Product results are divided into manageable pages where applicable.
* Customer can navigate between available result pages.
* The correct products are displayed when navigating between pages.

---

## CR-06 — Product Details

The marketplace shall allow customers to view detailed information about a product before purchase.

Product information may include:

* Product name
* Description
* Destination
* Price
* Images
* Availability / quantity
* Participant requirements
* Terms and conditions
* Other relevant product information

### Acceptance Criteria

* Customer can open a product.
* Relevant product information is displayed.
* Customer can proceed to add the product to the cart.

---

# 3. Recommendation & Cross-Sell Requirements

## CR-07 — Destination-Based Recommendations

The marketplace should be capable of surfacing relevant products based on the customer's travel journey.

For example, a customer interested in travelling to a particular destination may be shown relevant:

* Tours
* Activities
* Hotels
* Concierge services
* Other destination-related products

### Acceptance Criteria

* Relevant destination information can be associated with products.
* The platform can identify products associated with the customer's journey or destination.
* Relevant products can be surfaced as recommendations.

The objective is to create additional product discovery and cross-selling opportunities.

---

# 4. Vendor Requirements

## VR-01 — Vendor Registration

The marketplace shall allow external travel providers to register as vendors.

### Acceptance Criteria

* Vendor can access the registration process.
* Vendor can provide required registration information.
* Successful registration creates a vendor account.
* Vendor can subsequently access vendor functionality.

---

## VR-02 — Product Creation

The marketplace shall allow approved vendors and internal product owners to create products.

### Acceptance Criteria

* Vendor can initiate product creation.
* Vendor can provide required product information.
* Vendor can specify relevant pricing and availability information.
* Vendor can upload product images.
* Vendor can save or submit the product according to the available workflow.

---

## VR-03 — Product Submission

The marketplace shall allow vendors to submit completed products for review.

### Acceptance Criteria

* Vendor can submit a completed product.
* Submitted products enter a review status.
* Product is not publicly available before approval.

---

# 5. Product Governance Requirements

## GR-01 — Product Approval

The marketplace shall provide a central product approval process managed by the Marketplace Administrator.

### Acceptance Criteria

* Submitted products appear in the administrator's review queue.
* Administrator can review submitted product information.
* Administrator can approve a product.
* Approved products can proceed to publication.

---

## GR-02 — Product Rejection

The Marketplace Administrator shall be able to decline products that do not meet approved marketplace guidelines.

### Acceptance Criteria

* Administrator can decline a submitted product.
* Administrator can provide a reason or feedback.
* Declined products are not published.
* Vendor or product owner can update the product and resubmit it.

---

## GR-03 — Product Visibility

Only approved products shall be available for customer discovery.

### Acceptance Criteria

* Draft products are not publicly visible.
* Submitted products awaiting approval are not publicly visible.
* Declined products are not publicly visible.
* Approved products can become available according to marketplace publication rules.

---

# 6. Product Boosting Requirements

## BR-01 — Product Boosting

The marketplace shall allow vendors or product owners to pay for increased product visibility.

### Acceptance Criteria

* Vendor can choose whether to boost a product.
* Boosting attracts an additional fee.
* A successfully boosted and approved product receives higher search placement.
* Vendors can also access the boost option for eligible existing products.

---

## BR-02 — Organic Product Visibility

Products that are approved but not boosted shall remain eligible for normal marketplace visibility.

### Acceptance Criteria

* Non-boosted approved products remain searchable.
* Approval does not require payment for boosting.
* Paid boosting is treated as an additional visibility option rather than a requirement for publication.

---

# 7. Cart Requirements

## CART-01 — Add Product to Cart

The marketplace shall allow customers to add products to a shopping cart.

### Acceptance Criteria

* Customer can add an available product to the cart.
* Selected product appears in the cart.
* Relevant quantity and pricing information is displayed.

---

## CART-02 — Multiple Products

The marketplace shall allow customers to add multiple products to the same cart.

Examples include:

* Flight + Hotel
* Flight + Tour
* Flight + Hotel + Tour
* Tour + Airport Concierge
* Multiple travel-related services

### Acceptance Criteria

* Customer can add multiple eligible products.
* Cart displays all selected products.
* Cart calculates the applicable purchase total.
* Customer can review the combined purchase before checkout.

---

# 8. Checkout & Payment Requirements

## PAY-01 — Unified Checkout

The marketplace shall provide a central checkout process for products purchased through the platform.

### Acceptance Criteria

* Customer can review all selected products.
* Customer can proceed from cart to checkout.
* Customer is not required to initiate separate checkout journeys for products contained within the same cart.

---

## PAY-02 — Online Payment

The marketplace shall allow customers to complete payment online through the platform.

### Acceptance Criteria

* Customer can initiate payment.
* Successful payment is recorded.
* Failed payment is appropriately communicated.
* Payment status is associated with the relevant transaction.

---

## PAY-03 — Purchase Confirmation

The marketplace shall provide confirmation after successful purchase.

### Acceptance Criteria

* Successful transaction generates a purchase confirmation.
* Customer receives confirmation through the configured notification channel.
* Relevant vendor or internal product owner is notified.

---

# 9. Inventory & Availability Requirements

## INV-01 — Product Quantity

The marketplace shall support quantity or availability information for products where applicable.

### Acceptance Criteria

* Vendor can specify available quantity where required.
* Available quantity is displayed to the customer where applicable.
* Purchase reduces available quantity accordingly.

---

## INV-02 — Minimum Participant Requirement

The marketplace shall support products with minimum participation requirements.

### Acceptance Criteria

* Vendor can define the minimum participant requirement where applicable.
* Relevant booking information is retained.
* Vendor can determine whether to proceed where the minimum requirement is not met by the applicable deadline.

---

# 10. Notification Requirements

## NOT-01 — Customer Notification

The marketplace shall notify customers following relevant transaction events.

Examples include:

* Successful purchase
* Purchase confirmation
* Relevant cancellation or exception events

---

## NOT-02 — Vendor Notification

The marketplace shall notify the responsible vendor or internal product owner when a purchase is completed.

The notification should provide the information required for fulfilment.

---

# 11. Vendor Fulfilment Requirements

## FUL-01 — Traveller Information

The responsible vendor or internal product owner shall have access to relevant traveller information required to fulfil a purchased product.

This may include:

* Customer name
* Contact details
* Product purchased
* Quantity
* Payment status
* Booking date
* Number of participants
* Traveller details
* Fulfilment status

---

## FUL-02 — Fulfilment Status

The marketplace shall support visibility into the fulfilment status of purchased products.

The responsible vendor or product owner remains responsible for fulfilment.

---

# 12. Cancellation & Voucher Requirements

## CAN-01 — Product Cancellation

Where a product cannot proceed because of a product-specific condition, the marketplace shall support the applicable cancellation process.

For example, a tour may not proceed if the minimum required number of participants is not reached.

---

## CAN-02 — Customer Voucher

Where applicable under the marketplace terms and conditions, a cancelled purchase may result in a voucher equivalent to the refunded amount.

### Acceptance Criteria

* Eligible cancelled purchases are identified.
* Applicable refund/voucher value is calculated.
* Customer receives the applicable voucher.
* Voucher can be applied toward another eligible marketplace product.

---

# 13. Marketplace Administration Requirements

## ADM-01 — Product Management

The Marketplace Administrator shall be able to monitor and manage submitted marketplace products.

---

## ADM-02 — Product Approval Queue

The administrator shall be able to view products requiring review.

The dashboard should provide visibility into:

* Total products uploaded
* Pending approvals
* Declined products
* Other relevant product statuses

---

## ADM-03 — Marketplace Sales Reporting

The administrator shall be able to monitor marketplace sales.

Reporting should support analysis such as:

* Total sales
* Sales by vendor
* Sales by destination
* Top destination
* Top vendor
* Gross revenue

---

## ADM-04 — Vendor Statements

The marketplace should allow the administrator to generate a statement of account for an individual vendor.

---

# 14. Vendor Dashboard Requirements

## VEN-01 — Vendor Performance

The vendor dashboard shall provide visibility into the performance of vendor products.

The dashboard should include:

* Product views
* Purchases
* Total revenue earned
* Amount spent on product boosting

Conversion rate was identified as a potential Phase 2 enhancement.

---

# 15. Executive Reporting Requirements

## EXEC-01 — Executive Dashboard

Management shall have access to a high-level marketplace performance view.

The dashboard should provide visibility into:

* Revenue from internally uploaded products
* Revenue generated by external vendors
* Customer growth
* Customers directed to the main BTM Holidays website
* Vendor growth
* New vendor registrations
* Platform performance
* Return on investment

The executive dashboard should focus on business performance and commercial outcomes rather than only operational activity.

---

# 16. Requirement Prioritisation

The requirements can be grouped into three broad delivery priorities.

### Core Marketplace

These capabilities form the foundation of the marketplace:

* Customer registration and login
* Product categories
* Product search
* Product details
* Vendor registration
* Product creation
* Product approval
* Product publication
* Cart
* Multiple products
* Checkout
* Online payment
* Notifications
* Quantity / availability
* Fulfilment

### Commercial Marketplace

These capabilities support marketplace monetisation and commercial management:

* Product boosting
* Vendor revenue reporting
* Internal vs external revenue reporting
* Vendor statements
* Executive revenue reporting

### Enhancement / Phase 2

These capabilities were identified as potential enhancements:

* Conversion-rate analytics
* More advanced recommendation capabilities
* Additional marketplace performance analytics

---

# BA Traceability

The requirements were derived from the underlying business objectives:

| Business Objective                        | Requirement Area                   |
| ----------------------------------------- | ---------------------------------- |
| Diversify revenue beyond flights          | Marketplace products               |
| Attract external providers                | Vendor onboarding                  |
| Maintain product quality                  | Marketplace approval               |
| Create additional commercial revenue      | Product boosting                   |
| Improve customer convenience              | Unified cart and checkout          |
| Increase cross-selling                    | Destination recommendations        |
| Support product owners                    | Vendor dashboards                  |
| Maintain fulfilment ownership             | Vendor fulfilment                  |
| Monitor marketplace performance           | Executive reporting                |
| Measure internal vs external contribution | Revenue reporting                  |
| Scale marketplace supply                  | Shared marketplace operating model |

---

## BA Perspective

The requirements were deliberately structured around **business outcomes, user journeys, operational responsibilities, and measurable platform behaviour**.

The goal was not simply to document features.

The goal was to translate the marketplace strategy into requirements that could be:

**understood → developed → tested → measured.**
