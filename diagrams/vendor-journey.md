# Vendor Journey

This flow illustrates how internal departments and external vendors submit products to the marketplace, obtain approval, and manage customer bookings.

```mermaid
graph TD
    A[Vendor Registers or Signs In] --> B[Create Product Listing]
    B --> C[Add Description and Images]
    C --> D[Submit Product for Review]
    D --> E[Marketplace Admin Reviews Product]
    E --> F{Approved?}
    F -->|No| G[Receive Rejection Feedback]
    G --> H[Correct Product Details]
    H --> D
    F -->|Yes| I[Product Published]
    I --> J{Boost Product?}
    J -->|Yes| K[Pay Boosting Fee]
    K --> L[Product Receives Boosted Placement]
    J -->|No| M[Standard Marketplace Placement]
    L --> N[Receive Booking Notification]
    M --> N
    N --> O[Review Booking and Customer Details]
    O --> P[Manage Fulfilment]
    P --> Q[Update Fulfilment Status]
```

## Key Business Rules

* Internal and external providers follow the same core product approval rules.
* Products must be approved before publication.
* Rejected products receive feedback so vendors can make corrections and resubmit.
* Paid boosting is optional and distinct from standard product placement.
* Vendors or responsible internal departments manage bookings and fulfilment after purchase.
