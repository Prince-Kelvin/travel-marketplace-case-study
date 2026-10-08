# UAT Test Scenarios & Results

## Purpose

The User Acceptance Testing (UAT) process was used to validate that the marketplace solution supported the agreed business requirements and end-to-end customer, vendor, administrative, and commercial workflows.

Testing focused on whether the solution met the intended business outcomes rather than only whether individual technical components functioned.

> **Portfolio note:** Test scenarios are presented at a business-process level. Confidential production data, payment information, customer information, and company-specific credentials have been excluded.

---

## UAT Approach

The UAT scope covered five major areas:

1. **Customer Experience**
2. **Vendor & Product Management**
3. **Marketplace Governance**
4. **Transaction & Fulfilment**
5. **Reporting & Business Performance**

The core validation approach was:

**Requirement → Test Scenario → Expected Business Outcome → Result → Defect/Observation → Retest → Acceptance**

---

# 1. Customer Experience

| ID     | Test Scenario                                          | Expected Result                                                                           | Result |
| ------ | ------------------------------------------------------ | ----------------------------------------------------------------------------------------- | ------ |
| UAT-01 | Register using supported customer registration methods | Customer account is successfully created using the available registration method.         | Passed |
| UAT-02 | Log in with a registered customer account              | Customer is authenticated and granted access to the appropriate marketplace experience.   | Passed |
| UAT-03 | Browse marketplace product categories                  | Customer can access the available marketplace categories and view relevant products.      | Passed |
| UAT-04 | Search/browse for a marketplace product                | Relevant marketplace products are presented for customer discovery.                       | Passed |
| UAT-05 | Navigate through multiple product pages                | Customer can move between product pages without losing the browsing experience.           | Passed |
| UAT-06 | Select a marketplace product                           | Customer is taken to the product details page and can review the product before purchase. | Passed |
| UAT-07 | Discover products relevant to a destination/journey    | Relevant destination-related products can be surfaced to the customer.                    | Passed |

---

# 2. Vendor & Product Management

| ID     | Test Scenario                                          | Expected Result                                                                                          | Result |
| ------ | ------------------------------------------------------ | -------------------------------------------------------------------------------------------------------- | ------ |
| UAT-08 | Register/onboard as a marketplace vendor               | Vendor registration information is captured and vendor can proceed through the onboarding process.       | Passed |
| UAT-09 | Create a new marketplace product                       | Vendor can enter the required product information and create a product listing.                          | Passed |
| UAT-10 | Upload product information and submit for approval     | Product is submitted into the marketplace approval workflow and is not immediately exposed to customers. | Passed |
| UAT-11 | Marketplace administrator approves a submitted product | Approved product becomes eligible for marketplace visibility.                                            | Passed |
| UAT-12 | Marketplace administrator rejects a submitted product  | Product is rejected and the vendor receives appropriate feedback/reason for the rejection.               | Passed |
| UAT-13 | Verify customer visibility after approval              | Approved products are visible to customers while unapproved products remain unavailable to customers.    | Passed |
| UAT-14 | Boost a product during product creation                | Vendor can select the boost option and the applicable boosting process is initiated.                     | Passed |
| UAT-15 | Boost an existing live product                         | Vendor can apply a boost to an already approved/live product.                                            | Passed |

---

# 3. Cart, Checkout & Payment

| ID     | Test Scenario                        | Expected Result                                                                            | Result |
| ------ | ------------------------------------ | ------------------------------------------------------------------------------------------ | ------ |
| UAT-16 | Add a marketplace product to cart    | Selected product is added to the customer's cart.                                          | Passed |
| UAT-17 | Add multiple products to cart        | Customer can combine multiple eligible marketplace products in the same shopping journey.  | Passed |
| UAT-18 | Proceed to unified checkout          | Customer can review selected products and proceed through a consolidated checkout process. | Passed |
| UAT-19 | Complete payment through the website | Payment is processed through the approved website payment flow.                            | Passed |
| UAT-20 | Complete a successful purchase       | Customer receives purchase confirmation and the transaction is recorded appropriately.     | Passed |

---

# 4. Inventory, Availability & Fulfilment

| ID     | Test Scenario                                       | Expected Result                                                                                     | Result |
| ------ | --------------------------------------------------- | --------------------------------------------------------------------------------------------------- | ------ |
| UAT-21 | Purchase a product with limited quantity/capacity   | Product quantity is reduced appropriately following a successful purchase.                          | Passed |
| UAT-22 | Attempt to purchase based on product availability   | Marketplace reflects the product's available quantity/capacity appropriately.                       | Passed |
| UAT-23 | Verify traveller information after purchase         | Relevant customer/traveller information is made available to the responsible vendor for fulfilment. | Passed |
| UAT-24 | Update fulfilment status                            | Vendor/internal product owner can manage and update the fulfilment status of the booking.           | Passed |
| UAT-25 | Handle product cancellation scenario                | Cancellation follows the applicable marketplace business rules and terms.                           | Passed |
| UAT-26 | Issue alternative value after eligible cancellation | Customer receives the applicable voucher/value following an eligible cancellation scenario.         | Passed |

---

# 5. Marketplace Administration & Reporting

| ID     | Test Scenario                               | Expected Result                                                                                                                          | Result |
| ------ | ------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------- | ------ |
| UAT-27 | Review marketplace product management area  | Marketplace administrator can view and manage products through the appropriate administrative workflow.                                  | Passed |
| UAT-28 | Review pending product approvals            | Administrator can identify products awaiting approval and take the appropriate action.                                                   | Passed |
| UAT-29 | Review marketplace sales reporting          | Marketplace sales information can be reviewed by relevant business dimensions such as vendor and destination.                            | Passed |
| UAT-30 | Generate/review vendor statement of account | Relevant vendor transaction information can be used to support vendor statement generation.                                              | Passed |
| UAT-31 | Review vendor performance information       | Vendor performance information such as purchases/revenue and relevant marketplace activity can be reviewed.                              | Passed |
| UAT-32 | Review executive marketplace dashboard      | Management can review marketplace performance information including revenue, customer growth, vendor growth, and ROI-related indicators. | Passed |

---

# UAT Result Summary

| Area                        | Scenarios | Passed | Failed | Status       |
| --------------------------- | --------: | -----: | -----: | ------------ |
| Customer Experience         |         7 |      7 |      0 | Accepted     |
| Vendor & Product Management |         8 |      8 |      0 | Accepted     |
| Cart, Checkout & Payment    |         5 |      5 |      0 | Accepted     |
| Inventory & Fulfilment      |         6 |      6 |      0 | Accepted     |
| Administration & Reporting  |         6 |      6 |      0 | Accepted     |
| **Total**                   |    **32** | **32** |  **0** | **Accepted** |

---

# Representative UAT Scenarios

## Scenario 1 — Product Approval & Visibility

**Objective:**
Validate that marketplace products cannot become customer-visible before completing the approval process.

**Given:**

* A vendor has created a marketplace product.
* The product has been submitted for review.

**When:**

* The Marketplace Administrator reviews and approves the product.

**Then:**

* The product becomes eligible for customer visibility.
* The product can appear in marketplace discovery.
* The vendor can proceed with marketplace selling activities.

**Business Value:**
Protects marketplace quality and establishes consistent governance across internal and external products.

---

## Scenario 2 — Multiple Products in One Customer Journey

**Objective:**
Validate that a customer can combine different travel services within one purchase journey.

**Given:**

* A customer is searching for travel-related products.

**When:**

* The customer selects multiple eligible products, such as a flight, hotel, tour, or concierge service.
* The customer adds them to the cart.

**Then:**

* The products remain available within the same cart.
* The customer can proceed to a unified checkout experience.

**Business Value:**
Creates opportunities to increase basket value by allowing customers to purchase complementary travel services within one journey.

---

## Scenario 3 — Product Capacity & Purchase

**Objective:**
Validate that product availability is appropriately managed after purchase.

**Given:**

* A product has a defined quantity or participant capacity.

**When:**

* A customer purchases the product.

**Then:**

* The purchased quantity is reflected in the marketplace.
* Remaining availability is appropriately maintained.
* The vendor receives the relevant purchase information for fulfilment.

**Business Value:**
Reduces the risk of overselling and provides vendors with the information required to fulfil customer bookings.

---

## Scenario 4 — Minimum Participant Requirement

**Objective:**
Validate the business process for products requiring a minimum number of participants.

**Given:**

* A tour has a minimum participant requirement.
* The booking deadline has been reached.

**When:**

* The minimum participant threshold has not been met.

**Then:**

* The vendor determines whether to proceed with the tour.
* If the vendor does not proceed, the applicable cancellation process is initiated.
* The customer receives the applicable voucher/value according to the marketplace terms.

**Business Value:**
Provides a defined process for handling group-based products where fulfilment depends on reaching a minimum participant threshold.

---

# UAT Defect & Observation Handling

Where a test did not produce the expected business outcome, the issue was assessed based on its impact on the customer journey or business process.

The general process was:

**Test → Identify Issue → Document Observation → Assign/Discuss → Fix → Retest → Accept**

Issues were evaluated based on factors such as:

* Customer impact
* Transaction impact
* Business-rule impact
* Operational impact
* Reporting impact
* Severity and priority

---

# Business Acceptance Criteria

The marketplace was considered ready for business acceptance when the agreed critical business journeys could be successfully demonstrated across:

* Customer registration and authentication
* Product discovery
* Product details
* Vendor onboarding
* Product submission
* Product approval and rejection
* Marketplace visibility
* Product boosting
* Cart and multi-product purchase
* Website payment
* Purchase confirmation
* Quantity and availability
* Vendor fulfilment
* Cancellation and voucher handling
* Marketplace administration
* Management reporting

---

## BA Contribution

My role in UAT extended beyond executing test cases.

I translated business requirements into testable scenarios, coordinated validation across different marketplace workflows, reviewed expected business outcomes, identified gaps between requirements and actual behaviour, and supported the transition from requirements validation to business acceptance.

This ensured that UAT focused on a critical question:

> **Can the business actually operate the marketplace successfully from customer discovery through fulfilment and reporting?**

---

## Key Takeaway

The UAT process demonstrated the importance of validating an entire business journey rather than testing isolated features.

For this marketplace, successful acceptance required the following chain to work together:

**Discover → Select → Cart → Pay → Confirm → Fulfil → Report**

That end-to-end perspective helped ensure that the marketplace was evaluated as a **business product**, not simply as a collection of software features.
