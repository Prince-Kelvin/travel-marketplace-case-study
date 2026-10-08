# Marketplace User Stories & Acceptance Criteria

## Purpose

The user stories translated the marketplace requirements into user-centred, testable backlog items.

The stories were structured around the major marketplace actors:

* Customer
* External Vendor
* Internal Product Owner
* Marketplace Administrator
* Executive Management

Each story follows the standard Agile format:

> **As a [user], I want [capability], so that [business value].**

Acceptance criteria define the expected behaviour and provide a foundation for development and UAT.

---

# Epic 1 — Customer Registration & Access

## US-01 — Customer Registration

**As a customer,**
I want to register on the marketplace using a supported registration method,
**so that I can access marketplace services and complete purchases.**

### Acceptance Criteria

* Customer can register using Google.
* Customer can register using Facebook.
* Customer can register using email.
* Customer can register using phone number.
* Successful registration creates a customer account.
* Registration errors are communicated clearly.

---

## US-02 — Customer Login

**As a registered customer,**
I want to log into my account,
**so that I can access the marketplace as an authenticated user.**

### Acceptance Criteria

* Valid authentication details allow login.
* Invalid details prevent login.
* Appropriate feedback is displayed when authentication fails.

---

# Epic 2 — Product Discovery

## US-03 — Browse Product Categories

**As a customer,**
I want to browse products by category,
**so that I can quickly find the type of travel service I need.**

### Acceptance Criteria

* Product categories are displayed.
* Categories include applicable marketplace offerings.
* Selecting a category displays relevant products.
* Products displayed belong to the selected category.

---

## US-04 — Search for Products

**As a customer,**
I want to search for marketplace products,
**so that I can find relevant travel services.**

### Acceptance Criteria

* Customer can enter a search query.
* Relevant products are returned.
* Search results can be browsed.
* No-result scenarios provide appropriate feedback.

---

## US-05 — Navigate Product Results

**As a customer,**
I want product results to be paginated,
**so that I can browse a large catalogue without being overwhelmed by one long page.**

### Acceptance Criteria

* Results are divided into pages where applicable.
* Customer can navigate between pages.
* Correct products are displayed for each page.
* Customer can identify the current result position where applicable.

---

## US-06 — View Product Details

**As a customer,**
I want to view detailed information about a product,
**so that I can make an informed purchase decision.**

### Acceptance Criteria

Product details may include:

* Product name
* Description
* Destination
* Price
* Images
* Availability / quantity
* Participant requirements
* Terms and conditions

Customer can add the product to the cart from the product detail experience.

---

# Epic 3 — Recommendation & Cross-Selling

## US-07 — Discover Relevant Destination Products

**As a traveller,**
I want to see relevant products associated with my destination,
**so that I can discover additional services that may be useful during my trip.**

### Acceptance Criteria

* Products can be associated with destinations.
* Destination context can be used to identify relevant products.
* Relevant products can be surfaced to the customer.
* Recommendations support additional product discovery.

---

# Epic 4 — Vendor Onboarding & Product Management

## US-08 — Register as a Vendor

**As an external travel provider,**
I want to register as a marketplace vendor,
**so that I can offer my products to marketplace customers.**

### Acceptance Criteria

* Provider can access vendor registration.
* Provider can submit required information.
* Successful registration creates a vendor account.
* Registered vendor can access vendor functionality.

---

## US-09 — Create a Product

**As a vendor,**
I want to create a marketplace product,
**so that I can make my travel offering available for review.**

### Acceptance Criteria

Vendor can provide applicable product information including:

* Product name
* Description
* Destination
* Price
* Availability
* Quantity
* Images
* Participant requirements
* Terms and conditions

Vendor can submit the completed product for review.

---

## US-10 — Upload Product Images

**As a vendor,**
I want to upload product images,
**so that customers can visually understand the product before purchasing.**

### Acceptance Criteria

* Vendor can upload applicable product images.
* Images are associated with the correct product.
* Images are available for review before publication.

---

## US-11 — Submit Product for Approval

**As a vendor,**
I want to submit my completed product for approval,
**so that it can be reviewed before being published.**

### Acceptance Criteria

* Completed product can be submitted.
* Product status changes to a review state.
* Product is not publicly visible before approval.
* Vendor can identify the product's current status.

---

# Epic 5 — Product Governance

## US-12 — Review Product

**As a Marketplace Administrator,**
I want to review submitted products,
**so that only products meeting marketplace guidelines are published.**

### Acceptance Criteria

* Administrator can access submitted products.
* Administrator can review product information.
* Administrator can approve an eligible product.
* Administrator can decline a product that does not meet requirements.

---

## US-13 — Provide Rejection Feedback

**As a Marketplace Administrator,**
I want to provide a reason when declining a product,
**so that the vendor understands what needs to be corrected.**

### Acceptance Criteria

* Administrator can enter rejection feedback.
* Declined product remains unpublished.
* Vendor can view the feedback.
* Vendor can update the product.
* Updated product can be resubmitted.

---

## US-14 — Publish Approved Product

**As a Marketplace Administrator,**
I want approved products to become available for customer discovery,
**so that customers can purchase eligible marketplace products.**

### Acceptance Criteria

* Approved product becomes eligible for publication.
* Published product appears in applicable marketplace results.
* Product information displayed to customers reflects the approved submission.

---

# Epic 6 — Product Visibility & Boosting

## US-15 — Boost Product Visibility

**As a vendor,**
I want to pay to boost my product,
**so that it receives increased visibility within marketplace search.**

### Acceptance Criteria

* Vendor can select the boost option.
* Applicable additional fee is presented.
* Boost is applied only after the product satisfies normal approval requirements.
* Boosted product receives higher search placement.

---

## US-16 — Boost Existing Product

**As a vendor,**
I want to boost an existing live product,
**so that I can increase its visibility after publication.**

### Acceptance Criteria

* Eligible live products display the boost option.
* Vendor can initiate a boost.
* Applicable fee is processed.
* Successful boost increases product visibility.

---

# Epic 7 — Cart & Checkout

## US-17 — Add Product to Cart

**As a customer,**
I want to add a product to my cart,
**so that I can purchase it during checkout.**

### Acceptance Criteria

* Customer can add an available product.
* Product appears in the cart.
* Correct quantity and price are displayed.

---

## US-18 — Add Multiple Products

**As a customer,**
I want to add multiple travel products to one cart,
**so that I can manage related purchases together.**

### Acceptance Criteria

* Customer can add multiple eligible products.
* Cart displays all selected products.
* Each product retains its relevant quantity and price.
* Cart displays the applicable total.

---

## US-19 — Complete Unified Checkout

**As a customer,**
I want to complete my selected purchases through one checkout process,
**so that I do not have to manage separate payment journeys across different providers.**

### Acceptance Criteria

* Customer can review all cart items.
* Customer can proceed to checkout.
* Customer can complete the transaction through the marketplace.
* Successful payment produces a confirmed transaction.

---

# Epic 8 — Inventory & Purchase Processing

## US-20 — Maintain Product Quantity

**As a vendor,**
I want product availability to update after purchases,
**so that customers are not shown inaccurate availability.**

### Acceptance Criteria

* Product has an available quantity where applicable.
* Successful purchase reduces the available quantity.
* Updated quantity is reflected in the marketplace.

---

## US-21 — Enforce Availability

**As a customer,**
I want the marketplace to respect product availability,
**so that I cannot purchase unavailable capacity.**

### Acceptance Criteria

* Available products can be purchased.
* Products with no remaining capacity cannot be purchased as available.
* Appropriate availability information is displayed.

---

# Epic 9 — Notifications & Fulfilment

## US-22 — Receive Purchase Confirmation

**As a customer,**
I want to receive confirmation after successful payment,
**so that I know my purchase has been completed.**

### Acceptance Criteria

* Successful payment generates a purchase confirmation.
* Confirmation is sent through the configured notification channel.
* Purchase information is included as applicable.

---

## US-23 — Notify Vendor of Purchase

**As a vendor,**
I want to receive notification when my product is purchased,
**so that I can begin fulfilment.**

### Acceptance Criteria

* Vendor receives notification after successful purchase.
* Notification identifies the purchased product.
* Relevant customer and transaction information is available.

---

## US-24 — View Traveller Information

**As a vendor,**
I want access to relevant traveller information,
**so that I can fulfil the purchased service.**

### Acceptance Criteria

Vendor can access applicable:

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

## US-25 — Update Fulfilment Status

**As a vendor,**
I want to manage the fulfilment status of a purchase,
**so that the marketplace reflects the current state of the booking.**

### Acceptance Criteria

* Vendor can access relevant purchased products.
* Vendor can update fulfilment status.
* Updated status is available to authorised users.

---

# Epic 10 — Minimum Participation & Cancellation

## US-26 — Manage Minimum Participant Requirement

**As a vendor,**
I want to define a minimum participant requirement for applicable products,
**so that I can manage products that require a minimum number of travellers.**

### Acceptance Criteria

* Vendor can specify the minimum participant requirement.
* Requirement is associated with the product.
* Relevant booking information is available to the vendor.

---

## US-27 — Decide Whether Minimum-Participant Product Proceeds

**As a vendor,**
I want to determine whether a product proceeds when the minimum participant threshold is not met,
**so that I can make the operational decision based on the product's requirements.**

### Acceptance Criteria

* Vendor can identify whether the minimum requirement was achieved.
* Vendor can determine whether to proceed.
* Where the vendor elects not to proceed, the applicable cancellation process can begin.

---

## US-28 — Issue Customer Voucher

**As a customer affected by an eligible product cancellation,**
I want to receive a voucher equivalent to the applicable refunded amount,
**so that I can use the value toward another marketplace product.**

### Acceptance Criteria

* Eligible cancellation is identified.
* Applicable voucher value is calculated.
* Voucher is issued to the affected customer.
* Voucher can be applied to another eligible marketplace purchase.

---

# Epic 11 — Marketplace Administration & Reporting

## US-29 — Monitor Product Pipeline

**As a Marketplace Administrator,**
I want to see product submission statuses,
**so that I can manage the marketplace catalogue effectively.**

### Acceptance Criteria

Dashboard provides visibility into applicable statuses including:

* Total products uploaded
* Pending approvals
* Declined products

---

## US-30 — Monitor Marketplace Sales

**As a Marketplace Administrator,**
I want to monitor marketplace sales,
**so that I can understand commercial activity across the platform.**

### Acceptance Criteria

Reporting can provide:

* Total sales
* Sales by vendor
* Sales by destination
* Top destination
* Top vendor
* Gross revenue

---

## US-31 — Generate Vendor Statement

**As a Marketplace Administrator,**
I want to generate a statement of account for a vendor,
**so that vendor-level financial activity can be reviewed.**

### Acceptance Criteria

* Administrator can select a vendor.
* Applicable transaction information is retrieved.
* Vendor statement can be generated.

---

# Epic 12 — Vendor Performance

## US-32 — View Product Performance

**As a vendor,**
I want to see the performance of my products,
**so that I can understand how my marketplace offerings are performing.**

### Acceptance Criteria

Vendor dashboard can display:

* Product views
* Purchases
* Total revenue earned
* Amount spent on boosting

Conversion rate is treated as a potential Phase 2 enhancement.

---

# Epic 13 — Executive Management

## US-33 — Monitor Marketplace Business Performance

**As an executive,**
I want to view high-level marketplace performance,
**so that I can determine whether the marketplace is delivering business value.**

### Acceptance Criteria

Executive reporting provides visibility into:

* Revenue from internal products
* Revenue from external vendors
* Customer growth
* Customers directed to the main BTM Holidays website
* Vendor growth
* New vendor registrations
* Platform performance
* Return on investment

---

# User Story Prioritisation

The stories can be grouped using a practical delivery approach.

## Must Have — Marketplace Foundation

* Customer registration
* Customer login
* Product categories
* Product search
* Product pagination
* Product details
* Vendor registration
* Product creation
* Product submission
* Product approval
* Product rejection
* Product publication
* Cart
* Multiple products
* Unified checkout
* Online payment
* Purchase confirmation
* Vendor notification
* Quantity management
* Fulfilment

## Should Have — Commercial & Governance

* Product boosting
* Vendor performance dashboard
* Marketplace sales reporting
* Vendor statements
* Executive dashboard
* Destination-based recommendations
* Minimum participant rules
* Cancellation and voucher handling

## Phase 2 / Enhancement

* Conversion-rate analytics
* More advanced recommendation capabilities
* Additional marketplace performance analytics

---

# BA Traceability

The user stories provide a bridge between business requirements and UAT.

```text
Business Objective
        ↓
Requirement
        ↓
User Story
        ↓
Acceptance Criteria
        ↓
Development
        ↓
UAT Scenario
        ↓
Business Sign-off
```

This structure helped ensure that business expectations could be translated into delivery-ready requirements and subsequently validated during UAT.

---

## BA Perspective

The user stories were not treated simply as documentation.

They provided a common language between:

**Business → Product → Development → QA → UAT → Stakeholders**

The acceptance criteria also created a natural foundation for the later UAT scenarios and requirements traceability matrix.
