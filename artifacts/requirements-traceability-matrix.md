# Requirements Traceability Matrix

## Purpose

The Requirements Traceability Matrix (RTM) provides a structured link between the marketplace's business objectives, functional requirements, user stories, business rules, and UAT coverage.

The purpose of the matrix is to ensure that important business requirements are not lost between discovery, development, testing, and business validation.

---

## Traceability Model

The marketplace requirements follow this chain:

```text
Business Objective
       ↓
Requirement
       ↓
Business Rule / User Story
       ↓
Acceptance Criteria
       ↓
UAT Scenario
       ↓
Business Validation
```

---

# Requirements Traceability Matrix

| ID      | Business Need                                      | Requirement                  | User Story | Business Rule | UAT Coverage |
| ------- | -------------------------------------------------- | ---------------------------- | ---------- | ------------- | ------------ |
| CR-01   | Allow customers to access the marketplace          | Customer Registration        | US-01      | —             | UAT-01       |
| CR-02   | Allow registered customers to access their account | Customer Login               | US-02      | —             | UAT-02       |
| CR-03   | Help customers discover travel products            | Product Categories           | US-03      | —             | UAT-03       |
| CR-04   | Enable product discovery                           | Product Search               | US-04      | BR-23         | UAT-04       |
| CR-05   | Support large product catalogues                   | Product Pagination           | US-05      | —             | UAT-05       |
| CR-06   | Help customers make informed purchase decisions    | Product Details              | US-06      | BR-10         | UAT-06       |
| CR-07   | Increase relevant cross-selling                    | Destination Recommendations  | US-07      | BR-23         | UAT-07       |
| VR-01   | Expand marketplace supply                          | Vendor Registration          | US-08      | BR-18         | UAT-08       |
| VR-02   | Allow providers to contribute products             | Product Creation             | US-09      | BR-04         | UAT-09       |
| VR-03   | Control product publication                        | Product Submission           | US-11      | BR-01         | UAT-10       |
| GR-01   | Maintain catalogue quality                         | Product Approval             | US-12      | BR-01, BR-02  | UAT-11       |
| GR-02   | Provide governance feedback                        | Product Rejection            | US-13      | BR-02, BR-12  | UAT-12       |
| GR-03   | Prevent unapproved products from being visible     | Product Visibility           | US-14      | BR-01, BR-05  | UAT-13       |
| BR-01   | Create commercial visibility opportunities         | Product Boosting             | US-15      | BR-06         | UAT-14       |
| BR-02   | Allow ongoing product promotion                    | Existing Product Boost       | US-16      | BR-07         | UAT-15       |
| CART-01 | Support customer purchase                          | Add Product to Cart          | US-17      | BR-15         | UAT-16       |
| CART-02 | Allow bundled travel purchases                     | Multiple Products in Cart    | US-18      | BR-15         | UAT-17       |
| PAY-01  | Improve customer convenience                       | Unified Checkout             | US-19      | BR-14         | UAT-18       |
| PAY-02  | Enable marketplace transactions                    | Online Payment               | US-19      | BR-14         | UAT-19       |
| PAY-03  | Confirm completed purchases                        | Purchase Confirmation        | US-22      | BR-16         | UAT-20       |
| INV-01  | Manage capacity                                    | Product Quantity             | US-20      | BR-08         | UAT-21       |
| INV-02  | Prevent unavailable purchases                      | Availability Control         | US-21      | BR-09         | UAT-22       |
| FUL-01  | Support vendor fulfilment                          | Traveller Information        | US-24      | BR-16, BR-17  | UAT-23       |
| FUL-02  | Track service delivery                             | Fulfilment Status            | US-25      | BR-17         | UAT-24       |
| CAN-01  | Manage product-specific cancellation               | Product Cancellation         | US-27      | BR-11, BR-12  | UAT-25       |
| CAN-02  | Provide customer recovery option                   | Customer Voucher             | US-28      | BR-13         | UAT-26       |
| ADM-01  | Manage marketplace catalogue                       | Product Management           | US-29      | BR-01, BR-02  | UAT-27       |
| ADM-02  | Control product review pipeline                    | Approval Queue               | US-12      | BR-02         | UAT-28       |
| ADM-03  | Monitor commercial performance                     | Marketplace Sales Reporting  | US-30      | BR-20, BR-22  | UAT-29       |
| ADM-04  | Support vendor financial visibility                | Vendor Statement             | US-31      | BR-20         | UAT-30       |
| VEN-01  | Help vendors understand performance                | Vendor Performance Dashboard | US-32      | BR-21         | UAT-31       |
| EXEC-01 | Measure marketplace business value                 | Executive Dashboard          | US-33      | BR-20, BR-22  | UAT-32       |

---

# Business Objective Traceability

The RTM can also be viewed from the perspective of the original business objectives.

| Business Objective                        | Supporting Requirements          |
| ----------------------------------------- | -------------------------------- |
| Diversify revenue beyond flight bookings  | CR-03, VR-01, VR-02              |
| Attract external travel providers         | VR-01, VR-02, VR-03              |
| Maintain marketplace quality              | GR-01, GR-02, GR-03              |
| Create additional revenue from visibility | BR-01, BR-02                     |
| Improve customer convenience              | CART-01, CART-02, PAY-01, PAY-02 |
| Increase cross-selling                    | CR-04, CR-07                     |
| Support vendor fulfilment                 | FUL-01, FUL-02                   |
| Manage product capacity                   | INV-01, INV-02                   |
| Handle product-specific exceptions        | CAN-01, CAN-02                   |
| Monitor marketplace performance           | ADM-03, VEN-01, EXEC-01          |
| Measure internal vs external revenue      | ADM-03, EXEC-01                  |
| Evaluate return on investment             | EXEC-01                          |

---

# UAT Traceability

The UAT scenarios were structured to validate the major customer, vendor, administrative, and reporting workflows.

| UAT ID | Scenario                                   | Requirement Area       | Expected Validation                      |
| ------ | ------------------------------------------ | ---------------------- | ---------------------------------------- |
| UAT-01 | Register using Google                      | Customer Registration  | Account created successfully             |
| UAT-02 | Login with valid credentials               | Customer Login         | Customer authenticated                   |
| UAT-03 | Browse product category                    | Product Categories     | Relevant products displayed              |
| UAT-04 | Search for product                         | Product Search         | Relevant results returned                |
| UAT-05 | Navigate product pages                     | Pagination             | Correct result pages displayed           |
| UAT-06 | View product details                       | Product Details        | Required information displayed           |
| UAT-07 | View destination recommendations           | Recommendations        | Relevant products surfaced               |
| UAT-08 | Register vendor                            | Vendor Registration    | Vendor account created                   |
| UAT-09 | Create product                             | Product Creation       | Product saved/submitted                  |
| UAT-10 | Submit product                             | Product Submission     | Product enters review                    |
| UAT-11 | Approve product                            | Product Approval       | Product becomes eligible for publication |
| UAT-12 | Decline product                            | Product Rejection      | Feedback recorded                        |
| UAT-13 | Attempt to access unapproved product       | Product Visibility     | Product remains unavailable              |
| UAT-14 | Boost approved product                     | Product Boosting       | Higher visibility applied                |
| UAT-15 | Boost existing product                     | Existing Product Boost | Boost applied successfully               |
| UAT-16 | Add product to cart                        | Cart                   | Product appears in cart                  |
| UAT-17 | Add multiple products                      | Multi-product Cart     | Products appear together                 |
| UAT-18 | Complete unified checkout                  | Checkout               | Checkout completed                       |
| UAT-19 | Complete online payment                    | Payment                | Transaction recorded                     |
| UAT-20 | Receive purchase confirmation              | Notifications          | Customer receives confirmation           |
| UAT-21 | Purchase quantity-controlled product       | Quantity               | Quantity reduced                         |
| UAT-22 | Purchase unavailable product               | Availability           | Purchase prevented                       |
| UAT-23 | Vendor views traveller details             | Fulfilment             | Required information available           |
| UAT-24 | Update fulfilment status                   | Fulfilment             | Status updated                           |
| UAT-25 | Cancel product below minimum participation | Cancellation           | Applicable process triggered             |
| UAT-26 | Issue voucher                              | Customer Recovery      | Applicable voucher generated             |
| UAT-27 | Review marketplace products                | Admin Management       | Products visible to administrator        |
| UAT-28 | Manage approval queue                      | Governance             | Pending products identifiable            |
| UAT-29 | Review sales reporting                     | Reporting              | Sales data available                     |
| UAT-30 | Generate vendor statement                  | Vendor Reporting       | Statement generated                      |
| UAT-31 | Review vendor performance                  | Vendor Dashboard       | Performance metrics available            |
| UAT-32 | Review executive dashboard                 | Executive Reporting    | Strategic KPIs available                 |

---

# Traceability Coverage

The matrix provides coverage across the major marketplace domains:

### Customer

* Registration
* Authentication
* Search
* Categories
* Pagination
* Product details
* Recommendations
* Cart
* Checkout
* Payment
* Confirmation

### Vendor

* Registration
* Product creation
* Product submission
* Product visibility
* Boosting
* Quantity
* Purchases
* Traveller information
* Fulfilment
* Performance reporting

### Marketplace Administration

* Product approval
* Product rejection
* Feedback
* Approval queue
* Catalogue management
* Sales reporting
* Vendor statements

### Management

* Internal revenue
* External vendor revenue
* Customer growth
* Vendor growth
* New vendor registrations
* Platform performance
* ROI

---

# Traceability Gaps & Future Enhancements

The RTM also provides a mechanism for identifying requirements that may require further refinement.

Potential future areas include:

* More detailed recommendation rules
* Advanced conversion analytics
* Expanded vendor performance metrics
* More detailed cancellation workflows
* Additional payment exception scenarios
* Additional product-specific fulfilment rules

These areas can be added to the traceability matrix as the product evolves.

---

## BA Perspective

The RTM provides a single view of how the marketplace requirements connect across the delivery lifecycle.

It helps answer four critical questions:

1. **Why does this requirement exist?**
2. **What user need does it support?**
3. **What business rule governs it?**
4. **How will we validate it?**

This creates a direct connection between **strategy, requirements, Agile delivery, and UAT**.

For a Business Analyst, the value of the RTM is not the spreadsheet itself. The value is demonstrating that requirements remain connected to the business outcome they were created to achieve.
