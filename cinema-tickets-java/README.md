# Cinema Tickets

This is a coding exercise project that demonstrates an implementation of a `TicketService` for purchasing cinema tickets based on the given business rules, constraints, and assumptions.

## Business Rules

The following business rules apply to the ticket purchasing system:

- There are three types of tickets: Infant, Child, and Adult.

- Each ticket type has a corresponding price (see table below).

- The ticket purchaser specifies the number and type of tickets they want to buy.

- Multiple tickets can be purchased in a single transaction.

- A maximum of 20 tickets can be purchased at a time.

- Infants do not require a ticket and do not have a seat. They will be sitting on an adult's lap.

- Child and infant tickets cannot be purchased without an accompanying adult ticket.

| Ticket Type | Price |
|-------------|-------|
| INFANT      | £0    |
| CHILD       | £10   |
| ADULT       | £20   |

- The ticket purchasing system interacts with two external services:
    - `TicketPaymentService`: Responsible for processing payments.
    - `SeatReservationService`: Responsible for reserving seats.

## Constraints

The following constraints apply to the project:

- The `TicketService` interface cannot be modified (Java solution only).

- The code in the `thirdparty.*` packages cannot be modified.

- The `TicketTypeRequest` object should be immutable.

## Assumptions

The following assumptions are made for this project:

- All accounts with an ID greater than zero are considered valid and have sufficient funds to pay for any number of tickets.

- The `TicketPaymentService` implementation is an external provider without defects. The payment process itself is not a concern.

- Once a payment request is made to the `TicketPaymentService`, the payment will always be successful.

- The `SeatReservationService` implementation is an external provider without defects. The seat reservation algorithm is not a concern.

- Once a reservation request is made to the `SeatReservationService`, the seat will always be reserved successfully.


## Getting Started

To use the `TicketService` implementation, follow the steps below:

1. Clone the repository:
```
git clone https://github.com/mozbekler/cinema-tickets.git
```

2. Build and run the project.

3. Access the `TicketService` to purchase cinema tickets based on the provided functionality.

## Dependencies

The project has the following dependencies:

- `thirdparty.TicketPaymentService`: The external payment service for processing payments.

- `thirdparty.SeatReservationService`: The external service for reserving seats.

## Implementation Details

The implementation of the `TicketService` can be found in the project's source code. It takes into account the given business rules and requirements to provide a functional ticket purchasing system.

The code is designed to be clean, well-tested, and reusable. It follows best practices and ensures that the business rules are correctly met.

## Testing

Unit tests are provided
