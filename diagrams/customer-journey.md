# Customer Journey & Marketplace Experience

## Purpose

The marketplace was designed to allow travellers to discover and purchase multiple types of travel products through a single digital experience.

The customer journey was intentionally broader than traditional flight booking.

Instead of treating a flight as the end transaction, the marketplace could use the traveller's destination and journey intent to expose additional relevant products such as tours, hotels, airport concierge services, car hire, and activities.

---

## Customer Journey

The high-level customer journey was:

```text
Discover
   ↓
Search / Browse
   ↓
Explore Destination & Products
   ↓
View Product Details
   ↓
Select Product
   ↓
Add to Cart
   ↓
Continue Shopping
   ↓
Review Cart
   ↓
Checkout
   ↓
Online Payment
   ↓
Purchase Confirmation
   ↓
Vendor / Product Owner Notification
   ↓
Fulfilment
```

---

## 1. Discovery

The journey could begin outside the marketplace.

For example, a traveller searching online for information about a destination could discover the company's website.

A traveller interested in visiting a destination could then encounter relevant travel products available through the marketplace.

This created an opportunity to move from:

**Destination Interest → Product Discovery → Purchase**

rather than relying exclusively on customers who already intended to make a flight booking.

---

## 2. Search & Browse

Customers could browse the marketplace based on their travel needs.

Product categories included areas such as:

* Flights
* Tours
* Holiday packages
* Hotels
* Airport concierge / protocol services
* Car hire
* Fun and destination activities
* Study programmes
* Other travel-related services

The marketplace therefore supported both destination-led discovery and product-category discovery.

---

## 3. Destination-Based Cross-Selling

One of the opportunities identified during the product discovery process was to connect customer intent with relevant travel products.

For example:

```text
Traveller wants to visit Lagos
            ↓
Searches for / selects Lagos
            ↓
Relevant travel products surfaced
            ↓
Tours / Activities / Hotels / Concierge
            ↓
Traveller discovers additional services
```

Similarly, a traveller searching for or booking a flight to a destination could be exposed to relevant attractions, activities, tours, or other services available at that destination.

The objective was to encourage relevant cross-selling rather than treating every product as an isolated transaction.

---

## 4. Product Details

Before purchasing, the traveller could open a product and review its relevant information.

Depending on the product type, information could include:

* Product name
* Description
* Destination
* Price
* Availability / quantity
* Number of participants
* Product images
* Relevant terms and conditions
* Other product-specific information

The customer could then decide whether to add the product to the cart.

---

## 5. Multi-Product Cart

A key product decision was to allow travellers to add multiple products to one cart.

For example, a traveller could select:

```text
Flight
   +
Hotel
   +
Tour
   +
Airport Concierge
```

Rather than requiring the traveller to complete each purchase separately, the products could be managed through a unified cart experience.

This was important because travel purchases are often made up of multiple related services.

---

## 6. Unified Checkout

The marketplace used a central checkout experience.

The customer could:

1. Review selected products.
2. Confirm the purchase details.
3. Proceed to checkout.
4. Complete payment on the website.
5. Receive confirmation.

The product decision was deliberate: the traveller should not be required to move between multiple platforms or payment channels simply because the products came from different providers.

This created a more consistent customer experience while allowing different vendors to retain responsibility for fulfilment.

---

## 7. Purchase Confirmation

After successful payment, the customer received confirmation of the transaction.

The relevant vendor or internal product owner was also notified that a purchase had been made.

This allowed the fulfilment process to begin without requiring the customer to separately contact the provider to communicate that payment had been completed.

---

## 8. Fulfilment

After purchase, responsibility shifted from the central marketplace transaction layer to the relevant product owner.

For example:

```text
Customer purchases tour
        ↓
Marketplace confirms payment
        ↓
Tour owner receives notification
        ↓
Tour owner receives traveller details
        ↓
Tour fulfilment begins
```

The same principle applied to products managed by external vendors and internal departments.

---

## 9. Customer Journey Design Principle

The journey was built around three key principles:

### Discover More

Customers should be able to discover products beyond the service that initially brought them to the website.

### Buy in One Place

Customers should not have to manage multiple checkout and payment journeys for related travel products.

### Fulfil Through the Right Owner

The marketplace should manage the common transaction experience while the responsible vendor or internal product team manages fulfilment.

---

## End-to-End Journey

The complete experience can therefore be represented as:

```text
                 CUSTOMER JOURNEY

        ┌──────────────────────────┐
        │ Online / Destination     │
        │ Discovery                │
        └────────────┬─────────────┘
                     ↓
        ┌──────────────────────────┐
        │ Marketplace Search &     │
        │ Category Browsing        │
        └────────────┬─────────────┘
                     ↓
        ┌──────────────────────────┐
        │ Product / Destination    │
        │ Discovery                │
        └────────────┬─────────────┘
                     ↓
        ┌──────────────────────────┐
        │ Product Details          │
        └────────────┬─────────────┘
                     ↓
        ┌──────────────────────────┐
        │ Add to Cart              │
        │                          │
        │ Flight + Hotel + Tour   │
        │ + Concierge + Activities│
        └────────────┬─────────────┘
                     ↓
        ┌──────────────────────────┐
        │ Unified Checkout         │
        └────────────┬─────────────┘
                     ↓
        ┌──────────────────────────┐
        │ Online Payment           │
        └────────────┬─────────────┘
                     ↓
        ┌──────────────────────────┐
        │ Confirmation &           │
        │ Notifications            │
        └────────────┬─────────────┘
                     ↓
        ┌──────────────────────────┐
        │ Vendor / Internal Team   │
        │ Fulfilment               │
        └──────────────────────────┘
```

## BA/Product Insight

The key product insight was that the marketplace was not simply a catalogue of travel products.

It was designed as a **connected customer journey** in which an initial travel need could create opportunities for additional relevant purchases.

This shifted the product concept from:

> **"A website where customers can buy different travel products."**

to:

> **"A marketplace that connects customer travel intent with multiple relevant products through one purchasing journey."**

That distinction influenced the requirements around discovery, recommendations, cart functionality, checkout, notifications, and fulfilment.
