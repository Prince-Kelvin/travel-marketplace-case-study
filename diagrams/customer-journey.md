# Customer Journey

This flow illustrates how a customer discovers travel products, completes a booking, and receives fulfilment.

```mermaid
graph TD
    A[Visit Marketplace] --> B[Browse or Search Products]
    B --> C[View Product Details]
    C --> D{Suitable Product?}
    D -->|No| B
    D -->|Yes| E[Add to Cart]
    E --> F[Proceed to Checkout]
    F --> G[Pay on Marketplace Website]
    G --> H{Payment Successful?}
    H -->|No| F
    H -->|Yes| I[Booking Confirmation]
    I --> J[Notify Customer and Vendor]
    J --> K[Vendor Manages Fulfilment]
    K --> L[Booking Completed]
```

## Key Business Rules

* Customers can browse and search available travel products.
* Product details are available before booking.
* Payments are completed on the marketplace website.
* Successful payments trigger booking confirmation and notifications.
* The responsible vendor or internal department manages fulfilment.
