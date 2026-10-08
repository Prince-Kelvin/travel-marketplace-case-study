# Marketplace Business Rules

## Purpose

The marketplace business rules define the policies and decision logic governing how products, vendors, transactions, visibility, and fulfilment should operate.

Separating these rules from functional requirements makes the marketplace logic easier for product, engineering, QA, operations, and business stakeholders to understand and test.

---

# BR-01 — All Products Require Approval

No product shall become publicly visible on the marketplace until it has passed the required approval process.

**Rule:**

> A product must be reviewed and approved by the Marketplace Administrator before publication.

**Outcome:**

* Approved → eligible for publication
* Declined → not publicly visible

---

# BR-02 — Marketplace Administrator Provides Neutral Governance

Product approval shall be managed by the designated Marketplace Administrator rather than by individual product owners.

**Rule:**

> Product ownership does not give a department or vendor authority to approve its own product for marketplace publication.

**Purpose:**

This supports consistent governance and reduces the risk of preferential treatment.

---

# BR-03 — Internal and External Products Follow the Same Core Process

Internal departments and external vendors shall use the same core marketplace process.

**Rule:**

> Product ownership shall not create a separate approval, checkout, or customer journey.

Both internal and external products follow the same fundamental flow:

**Create → Submit → Review → Approve → Publish → Purchase → Fulfil**

---

# BR-04 — Product Ownership Remains With the Provider

Marketplace participation does not transfer operational ownership of a product to the central marketplace team.

**Rule:**

> The vendor or internal product owner remains responsible for the product and its fulfilment.

The marketplace provides the common transaction and governance framework.

---

# BR-05 — Approved Products Receive Normal Marketplace Visibility

Products that pass approval remain eligible for standard marketplace visibility.

**Rule:**

> Payment for boosting is not a prerequisite for product approval or publication.

This ensures that vendors can participate in the marketplace without being required to purchase additional visibility.

---

# BR-06 — Paid Boosting Provides Additional Visibility

A vendor or product owner may choose to pay for additional product visibility.

**Rule:**

> A boosted product receives higher search placement after meeting the normal product approval requirements.

Boosting does not bypass approval.

Therefore:

**Boosting ≠ Approval**

A product must still satisfy the marketplace's approval requirements.

---

# BR-07 — Existing Products Can Be Boosted

The boosting capability is not restricted to newly created products.

**Rule:**

> Eligible live products may be boosted after publication if the vendor or product owner chooses to purchase additional visibility.

This creates an ongoing commercial opportunity for the marketplace.

---

# BR-08 — Product Quantity Reduces After Purchase

Where a product has a defined quantity or capacity, a completed purchase shall reduce the available quantity.

**Rule:**

> Available quantity must be updated after a successful purchase.

Example:

```text
Available quantity = 20

Customer purchases 1

New available quantity = 19
```

This rule is particularly relevant for tours, activities, and other capacity-constrained products.

---

# BR-09 — Product Availability Must Be Respected

Customers should not be able to purchase a product when its available quantity has been exhausted.

**Rule:**

> A product with no remaining available capacity should not continue to be sold as available.

---

# BR-10 — Minimum Participant Rules Are Product-Specific

Some products may require a minimum number of participants before fulfilment can proceed.

**Rule:**

> Where a product has a minimum participant requirement, the requirement applies to that product and is managed by the responsible vendor or product owner.

Example:

```text
Minimum participants = 10
Booking deadline = 31 October
```

The marketplace records the relevant purchase and participant information, while the product owner determines whether the service can proceed where the minimum is not reached.

---

# BR-11 — Vendor Determines Whether a Minimum-Participant Product Proceeds

Where the minimum participant requirement is not met by the applicable deadline, the responsible vendor determines whether the product will proceed.

**Rule:**

> The platform does not automatically assume that the product must be cancelled solely because the minimum threshold was not reached.

The vendor may decide whether to proceed based on the product's operational requirements.

---

# BR-12 — Vendor-Initiated Cancellation Follows Terms & Conditions

If the vendor determines that a product cannot proceed, the cancellation must follow the applicable marketplace terms and conditions.

**Rule:**

> A vendor cannot independently create an alternative customer refund or cancellation process outside the agreed marketplace rules.

---

# BR-13 — Eligible Cancelled Purchases May Generate a Voucher

Where the applicable cancellation terms provide for a voucher, the customer receives a voucher equivalent to the refunded amount.

**Rule:**

> The voucher value should correspond to the applicable refunded amount.

The voucher may then be used toward another eligible marketplace product.

---

# BR-14 — Customer Payment Is Centralised

Customers should complete marketplace purchases through the central website checkout.

**Rule:**

> Customers should not be required to move to separate vendor platforms to complete payment for products purchased through the marketplace.

This supports the unified customer experience.

---

# BR-15 — Multiple Products Can Be Purchased Together

Customers may add multiple eligible products to the same cart.

**Rule:**

> The marketplace should support a combined purchasing journey for eligible products.

For example:

```text
Flight
+
Hotel
+
Tour
+
Airport Concierge
```

can form one customer cart.

---

# BR-16 — Vendor Receives Relevant Purchase Information

The responsible vendor or internal product owner receives the customer and transaction information required to fulfil the purchased product.

This can include:

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

# BR-17 — Fulfilment Responsibility Remains With Product Owner

The central marketplace is responsible for the marketplace transaction process, but not necessarily for operational fulfilment of every product.

**Rule:**

> The vendor or internal product owner remains responsible for delivering the purchased service.

---

# BR-18 — Internal Departments Can Operate as Vendors

Internal departments that own marketplace products may be treated as vendors within the marketplace operating model.

**Rule:**

> Internal product ownership does not require a separate marketplace process.

This allows the platform to maintain a consistent operating model across internal and external supply.

---

# BR-19 — Product-Specific Operational Rules Are Owned by the Product Owner

Different products may have different operational requirements.

**Rule:**

> Product-specific fulfilment decisions remain with the relevant product owner, provided they comply with marketplace policies and terms.

Examples may include:

* Minimum participants
* Availability
* Booking deadlines
* Fulfilment arrangements
* Product-specific conditions

---

# BR-20 — Marketplace Reporting Must Distinguish Supply Sources

Management reporting should distinguish between products supplied internally and products supplied by external vendors.

**Rule:**

> Marketplace reporting should allow revenue and performance to be analysed by supply source.

This supports management's need to understand the contribution of:

* Internal products
* External vendors

---

# BR-21 — Vendor Performance Is Measured Separately

Vendor reporting should allow individual vendors to understand their marketplace performance.

Relevant measures include:

* Product views
* Purchases
* Revenue earned
* Boosting spend

---

# BR-22 — Executive Reporting Focuses on Business Outcomes

Management reporting should focus on the commercial and strategic performance of the marketplace.

Key measures include:

* Internal product revenue
* External vendor revenue
* Customer growth
* Customers directed to the main BTM Holidays website
* Vendor growth
* New vendor registrations
* Platform performance
* Return on investment

---

# BR-23 — Recommendations Should Support Relevant Cross-Selling

Where recommendation logic is used, products should be surfaced based on the customer's travel journey or destination context.

**Rule:**

> Recommendations should be relevant to the customer's travel intent rather than being random product promotions.

For example:

```text
Flight to Destination
        ↓
Destination Identified
        ↓
Relevant Tours / Hotels / Activities
        ↓
Additional Product Discovery
```

---

# Business Rules Summary

| Rule  | Area              | Principle                                                      |
| ----- | ----------------- | -------------------------------------------------------------- |
| BR-01 | Governance        | Products require approval                                      |
| BR-02 | Governance        | Approval remains neutral                                       |
| BR-03 | Operating Model   | Internal and external products follow the same core process    |
| BR-04 | Ownership         | Product owner retains responsibility                           |
| BR-05 | Visibility        | Approved products receive normal visibility                    |
| BR-06 | Boosting          | Paid visibility does not bypass approval                       |
| BR-07 | Boosting          | Existing products can be boosted                               |
| BR-08 | Availability      | Purchase reduces quantity                                      |
| BR-09 | Availability      | Sold-out products cannot remain available                      |
| BR-10 | Product Rules     | Minimum participation can be product-specific                  |
| BR-11 | Fulfilment        | Vendor determines whether minimum-participant product proceeds |
| BR-12 | Cancellation      | Cancellation follows agreed terms                              |
| BR-13 | Customer Recovery | Eligible cancellations may generate vouchers                   |
| BR-14 | Payments          | Checkout is centralised                                        |
| BR-15 | Cart              | Multiple products can be purchased together                    |
| BR-16 | Fulfilment        | Vendor receives required traveller information                 |
| BR-17 | Fulfilment        | Product owner manages fulfilment                               |
| BR-18 | Vendors           | Internal teams can operate as vendors                          |
| BR-19 | Operations        | Product-specific rules remain with product owner               |
| BR-20 | Reporting         | Internal and external revenue are distinguishable              |
| BR-21 | Reporting         | Vendor performance is measurable                               |
| BR-22 | Reporting         | Executive reporting focuses on business outcomes               |
| BR-23 | Recommendations   | Cross-sell recommendations should be relevant                  |

---

## BA Perspective

The business rules establish the decision logic behind the marketplace.

They answer questions that functional requirements alone may not fully address:

* Who can approve a product?
* When can a product become visible?
* Can vendors pay to bypass approval?
* Who owns fulfilment?
* What happens when product capacity changes?
* Who decides whether a minimum-participant tour proceeds?
* What happens when a product is cancelled?
* How are internal and external products treated?
* What information does management need to evaluate the marketplace?

Documenting these rules separately creates a clearer bridge between **business policy, product behaviour, development, and UAT**.
