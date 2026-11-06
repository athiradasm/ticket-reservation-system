# Storyboard — Ticket Reservation System

## Purpose
Show the intended user journey from opening the application to managing a reservation.

## Actors
- **Guest:** browses available services.
- **Registered user:** books and manages tickets.
- **Administrator (planned):** manages schedules, inventory, and reservations.

## Storyboard sequence

### 1. Welcome / landing page
**Screen:** Application name, short description, and navigation.
**User action:** Selects Sign in, Register, or Search.
**System response:** Opens the selected page.

### 2. Registration and sign in
**Screen:** Registration form (name, email, password) and sign-in form.
**User action:** Creates an account or enters existing credentials.
**System response:** Validates input and opens the dashboard after successful authentication.
**Alternate path:** Invalid details produce a clear error message.

### 3. Search tickets
**Screen:** Search form with source/destination or event, date, and passenger count where relevant.
**User action:** Enters search criteria and submits.
**System response:** Displays matching options, times, prices, and availability.
**Alternate path:** If no results match, show a message and allow changed filters.

### 4. Select ticket / seat
**Screen:** Details of the chosen option and available seats or ticket quantity.
**User action:** Selects a seat or quantity.
**System response:** Shows the selection and calculated total before confirmation.
**Alternate path:** If inventory is no longer available, ask the user to choose again.

### 5. Review booking
**Screen:** Summary of service, date/time, passenger details, selected seats, and total price.
**User action:** Checks details and confirms or goes back to edit.
**System response:** Validates booking information.

### 6. Payment (planned integration)
**Screen:** Payment step or simulated payment page for a lab demo.
**User action:** Completes the approved test/sandbox flow.
**System response:** Records payment result. Never collect or store real card credentials in a student demo.

### 7. Booking confirmation
**Screen:** Confirmation message and booking reference.
**User action:** Views or saves confirmation.
**System response:** Stores reservation and makes it available in booking history.

### 8. My bookings / cancellation
**Screen:** List of upcoming and past bookings with status.
**User action:** Opens a booking or requests cancellation.
**System response:** Shows details and applies documented cancellation rules.

## Navigation flow

~~~mermaid
flowchart TD
    A[Welcome] --> B{Choose action}
    B --> C[Register / Sign in]
    C --> D[User dashboard]
    B --> E[Search tickets]
    D --> E
    E --> F{Results found?}
    F -->|No| E
    F -->|Yes| G[Select ticket / seat]
    G --> H[Review booking]
    H --> I[Payment or demo payment]
    I --> J[Confirmation]
    J --> K[My bookings]
    K --> L[View / cancel booking]
~~~

## Storyboard acceptance checks
- User can reach the search page.
- Search results reflect entered criteria.
- The selected ticket and total are visible before confirmation.
- A successful demo booking produces a unique reference.
- A user can view only their own bookings.
- Cancellation updates booking status according to project rules.
