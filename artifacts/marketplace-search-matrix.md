# Marketplace Search & Discovery Matrix

## Purpose

This matrix defines how customers discover marketplace products based on their travel needs, destinations, and product interests.

It translates customer intent into expected marketplace behaviour while maintaining clear traceability to business rules and UAT coverage.

> **Note:** The matrix intentionally avoids specifying technical search fields, filtering logic, sorting algorithms, or UI behaviour that were not explicitly defined during requirements gathering.

---

## Search & Discovery Matrix

| ID    | Customer Intent                                 | Discovery Entry Point              | Expected Marketplace Behaviour                                                                                                                                         | Result / Next Step                                                                                            | Business Rule | UAT Coverage   | Notes                                                                                |
| ----- | ----------------------------------------------- | ---------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------- | ------------- | -------------- | ------------------------------------------------------------------------------------ |
| SD-01 | Find a specific type of travel service          | Product category                   | Customer can browse available marketplace categories such as Flights, Hotels, Tours, Car Hire, Activities, Concierge/Protocol, Holiday Packages, and Study Programmes. | Customer selects a relevant category and views available products.                                            | BR-05         | UAT-03         | Category structure supports broad product discovery.                                 |
| SD-02 | Find products associated with a destination     | Destination-led discovery          | Marketplace can surface relevant products associated with the customer's travel destination or journey.                                                                | Customer discovers destination-relevant products such as hotels, tours, activities, or concierge services.    | BR-23         | UAT-07         | Supports cross-selling opportunities.                                                |
| SD-03 | Find a marketplace product                      | General product search             | Customer can search/browse marketplace products based on their travel requirement.                                                                                     | Matching products are presented for further exploration.                                                      | BR-23         | UAT-04         | Exact search-field behaviour remains implementation-dependent.                       |
| SD-04 | Browse a large number of products               | Product listing                    | Marketplace presents products in manageable pages rather than requiring the customer to navigate one continuous list.                                                  | Customer moves between pages to continue browsing.                                                            | —             | UAT-05         | Pagination improves product discoverability and usability.                           |
| SD-05 | Identify a product suitable for purchase        | Search/category results            | Customer selects a visible marketplace product from the available results.                                                                                             | Customer is taken to the product details page.                                                                | BR-05         | UAT-06         | Only approved products should be customer-visible.                                   |
| SD-06 | Understand a product before purchasing          | Product details                    | Customer can review relevant product information before adding the product to the cart.                                                                                | Customer decides whether to proceed with the purchase.                                                        | BR-10         | UAT-06         | Product detail content supports informed purchasing.                                 |
| SD-07 | Discover products relevant to a planned journey | Journey/destination recommendation | Marketplace can surface related products based on the customer's travel journey or destination.                                                                        | Customer can discover complementary services such as accommodation, activities, tours, or concierge services. | BR-23         | UAT-07         | Example: destination travel can lead to discovery of related activities or services. |
| SD-08 | Find products currently available for purchase  | Marketplace results                | Customer sees products that have passed marketplace approval and are available for customer purchase.                                                                  | Customer can proceed to product details and purchase where availability permits.                              | BR-01, BR-05  | UAT-13, UAT-22 | Unapproved products are not exposed to customers.                                    |
| SD-09 | Find highly visible marketplace products        | Marketplace search/results         | Approved products that have been boosted may receive higher placement within marketplace results.                                                                      | Customer may encounter boosted products earlier during discovery.                                             | BR-06, BR-07  | UAT-14, UAT-15 | Boosting affects placement, not approval status.                                     |
| SD-10 | Check whether a product can still be purchased  | Product details                    | Customer can view product availability/quantity where applicable.                                                                                                      | Customer can determine whether to proceed with the purchase.                                                  | BR-08, BR-09  | UAT-21, UAT-22 | Particularly relevant for products with limited capacity.                            |
| SD-11 | Continue exploring after viewing a product      | Product details → marketplace      | Customer can return to marketplace discovery after reviewing a product.                                                                                                | Customer can continue browsing other relevant products.                                                       | —             | UAT-06         | Supports multi-product purchase journeys.                                            |
| SD-12 | Combine different travel needs                  | Marketplace → Cart                 | Customer can discover and select multiple marketplace products that meet different parts of a journey.                                                                 | Selected products can be added to the cart for unified checkout.                                              | BR-15         | UAT-16, UAT-17 | Example: flight + hotel + tour + concierge.                                          |

---

## Discovery Principles

### 1. Category-led discovery

Marketplace categories provide a structured starting point for customers who know the type of service they need.

Examples include:

* Flights
* Hotels
* Tours
* Holiday Packages
* Car Hire
* Activities
* Airport Concierge/Protocol
* Study Programmes

### 2. Destination-led discovery

The marketplace is not limited to customers searching for a specific product.

A customer travelling to a destination can also be presented with relevant products associated with that journey.

For example:

**Travel destination → Hotel → Tour → Activity → Concierge service**

This creates an opportunity to increase the number of relevant products considered within a single customer journey.

### 3. Approval-controlled visibility

Search and discovery are governed by marketplace approval.

The discovery layer should only expose products that have passed the required marketplace approval process.

This creates a clear separation between:

**Product submitted → Product reviewed → Product approved → Product visible**

### 4. Organic visibility and paid boosting

Marketplace visibility has two distinct concepts:

* **Organic marketplace placement** — products are available based on normal marketplace discovery.
* **Paid boost** — a vendor can pay for increased visibility, causing an approved product to appear higher in marketplace results.

A boost does **not** bypass product approval.

### 5. Discovery should support conversion

Search and discovery are not treated as isolated features.

The intended journey is:

**Discover → Explore → Review → Add to Cart → Checkout → Purchase**

This connects marketplace discovery directly to the commercial objective of generating transactions.

---

## Search & Discovery Traceability

| Discovery Capability                 | Requirement | Business Rule | UAT    |
| ------------------------------------ | ----------- | ------------- | ------ |
| Product categories                   | CR-03       | —             | UAT-03 |
| Product search                       | CR-04       | BR-23         | UAT-04 |
| Pagination                           | CR-05       | —             | UAT-05 |
| Product details                      | CR-06       | BR-10         | UAT-06 |
| Destination recommendations          | CR-07       | BR-23         | UAT-07 |
| Approved product visibility          | GR-03       | BR-01, BR-05  | UAT-13 |
| Product boosting                     | BR-01       | BR-06         | UAT-14 |
| Existing product boosting            | BR-02       | BR-07         | UAT-15 |
| Product availability                 | INV-02      | BR-09         | UAT-22 |
| Multi-product discovery and purchase | CART-02     | BR-15         | UAT-17 |

---

## BA Observation

The marketplace search experience was designed around **customer intent rather than simply product listing**.

A customer may enter the marketplace knowing exactly what they want, such as a hotel or tour. Alternatively, they may begin with a destination and discover complementary products during the journey.

This distinction is important because the marketplace is intended not only to help customers find products, but also to create opportunities for **cross-selling, higher basket value, and increased marketplace revenue**.

> **Key BA principle:**
> **Make it easy for customers to find what they came for, while creating relevant opportunities to discover what they may also need.**
