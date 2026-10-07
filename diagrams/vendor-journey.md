# Vendor Journey & Product Lifecycle

## Purpose

The marketplace required a structured process for bringing products from vendors and internal product teams into the customer-facing catalogue.

The vendor journey was designed to balance two competing needs:

* Make it easy for providers to contribute products.
* Maintain sufficient governance over what customers could see and purchase.

The resulting lifecycle was:

```text
Vendor Registration
        ↓
Product Creation
        ↓
Product Information & Images
        ↓
Availability / Quantity
        ↓
Optional Product Boost
        ↓
Submit for Review
        ↓
Marketplace Administrator Review
        ↓
   ┌───────────────┐
   │               │
Approved        Declined
   │               │
   ↓               ↓
Published       Feedback
   │               │
   │               ↓
   │         Product Updated
   │               │
   │               ↓
   │          Resubmission
   │
   ↓
Customer Discovery
   ↓
Purchase
   ↓
Vendor Notification
   ↓
Fulfilment
```

---

## 1. Vendor Registration

External travel agencies and providers could register to participate in the marketplace.

The objective was to create a supply-side ecosystem rather than restricting the marketplace to products created by the company itself.

Internal departments could also participate as product owners.

This created two supply channels:

```text
Internal Product Owners ──┐
                          ├──> Marketplace
External Vendors ─────────┘
```

Both channels ultimately followed the same core product governance process.

---

## 2. Product Creation

After onboarding, the vendor or product owner could create a marketplace product.

The product creation process required relevant product information to be provided before submission.

Depending on the product type, this could include:

* Product name
* Product description
* Destination
* Pricing
* Availability
* Quantity
* Participant requirements
* Images
* Terms and conditions
* Other product-specific information

The purpose was to ensure that the marketplace had enough information for both governance and customer discovery.

---

## 3. Product Availability & Quantity

Products could have availability or quantity constraints.

For example, a tour product could specify:

* Number of available spaces
* Minimum participants
* Booking deadline

Once a customer purchased a product, the corresponding quantity was reduced in the system.

This prevented the marketplace from treating product availability as static information.

---

## 4. Product Images

Vendors could upload images as part of the product creation process.

Images supported the customer's product discovery and evaluation experience.

The product submission process therefore considered both structured product information and visual content.

---

## 5. Product Approval

A product was not automatically published after creation.

It first entered the marketplace approval process.

The Marketplace Administrator reviewed the submission against the approved marketplace guidelines.

The administrator could either:

### Approve

The product became eligible for publication and customer discovery.

### Decline

The product was rejected with a reason or feedback so that the vendor or product owner could make the necessary changes.

The product could then be updated and resubmitted.

---

## 6. Why a Dedicated Marketplace Administrator?

The dedicated Marketplace Administrator was an important governance decision.

Without a central administrator, individual teams could potentially influence which products received visibility based on internal relationships or ownership.

The proposed model created a neutral control point:

```text
Product Owner
     ↓
Marketplace Administrator
     ↓
Approval Decision
     ↓
Marketplace
```

The administrator's role was not to own the product.

It was to ensure that products entering the marketplace met the same basic standards.

This supported a more consistent and credible marketplace environment.

---

## 7. Product Visibility & Boosting

Once approved, products could receive normal marketplace visibility.

The marketplace also supported paid boosting.

A vendor could choose to pay an additional fee to increase product visibility.

### Standard Product

```text
Approved
   ↓
Normal Marketplace Visibility
```

### Boosted Product

```text
Approved
   ↓
Paid Boost
   ↓
Higher Search Placement
```

The same option could also be available to products that were already live.

This created an additional commercial revenue opportunity while keeping paid visibility separate from the basic approval process.

---

## 8. Product Purchase

Once published, the product became available to customers.

When a customer purchased the product:

1. The purchase was recorded.
2. The product quantity or availability was updated where applicable.
3. The customer received confirmation.
4. The responsible vendor or internal product owner received a notification.
5. The vendor or product owner began fulfilment.

---

## 9. Vendor Dashboard

Vendors required visibility into the commercial performance of their products.

The vendor dashboard included information such as:

* Product views
* Purchases
* Total revenue earned
* Amount spent on product boosting

Conversion rate was identified as a potential future enhancement rather than being treated as part of the initial dashboard scope.

This distinction helped keep the initial product scope focused while leaving room for future performance analytics.

---

## 10. Vendor Purchase Information

When a customer purchased a vendor's product, the vendor could access relevant transaction and traveller information required for fulfilment.

This included:

* Customer name
* Customer contact details
* Product purchased
* Quantity
* Payment status
* Booking date
* Number of participants
* Traveller details
* Fulfilment status

The purpose was to give the vendor sufficient information to complete the service without requiring the customer to repeat information through another channel.

---

## 11. Fulfilment

The marketplace handled the transaction layer, while the vendor or internal product owner remained responsible for fulfilment.

For example:

```text
Customer
   ↓
Purchases Product
   ↓
Marketplace
   ↓
Payment Confirmed
   ↓
Vendor Notified
   ↓
Vendor Receives Required Details
   ↓
Vendor Fulfilment
   ↓
Fulfilment Status Updated
```

This model allowed the marketplace to scale across different product categories without requiring the central marketplace team to operationally deliver every product.

---

## 12. Exception Handling

Some products had operational rules that could create exceptions after purchase.

For example, a tour could require a minimum number of participants.

If the minimum was not achieved by the deadline, the responsible vendor could determine whether the tour would proceed.

If the vendor decided not to proceed, the platform could support the cancellation process according to the applicable terms and conditions.

The affected customer could receive a voucher equivalent to the refunded amount for use toward another marketplace product.

This demonstrated the need for the marketplace to support both the standard purchase path and product-specific exceptions.

---

## Product Lifecycle Summary

The complete lifecycle can be represented as:

```text
                    PRODUCT LIFECYCLE

                 ┌──────────────┐
                 │    Draft     │
                 └──────┬───────┘
                        ↓
                 ┌──────────────┐
                 │  Submitted   │
                 └──────┬───────┘
                        ↓
              ┌────────────────────┐
              │ Marketplace Admin  │
              │      Review        │
              └─────────┬──────────┘
                        ↓
                ┌───────┴────────┐
                │                │
             Approved         Declined
                │                │
                ↓                ↓
          ┌───────────┐    ┌───────────┐
          │ Published │    │  Feedback │
          └─────┬─────┘    └─────┬─────┘
                │                │
                │                ↓
                │          Product Update
                │                │
                │                ↓
                │           Resubmission
                │                │
                │                └───────┐
                │                        │
                └────────────────────────┘
                         │
                         ↓
                    Customer
                    Purchase
                         │
                         ↓
                    Fulfilment
```

---

## BA/Product Insight

The vendor lifecycle highlighted an important marketplace design principle:

> **The marketplace should control the quality and transaction experience without taking ownership of every product's operational fulfilment.**

This separation allowed the platform to support multiple providers and product categories while maintaining a consistent customer experience.

It also created a foundation for marketplace scalability: more vendors and products could potentially be introduced without requiring the central marketplace team to directly fulfil every transaction.
