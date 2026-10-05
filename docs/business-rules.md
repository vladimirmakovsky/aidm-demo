# Business Rules

Every requirement must be checked against these rules. If a ticket contradicts a rule, the conflict must be raised with the Product Owner before development starts.

## Pricing and discounts

- **BR-01** All prices are shown and charged in EUR, VAT included.
- **BR-02** The order total can never be lower than 1.00 EUR after all discounts.
- **BR-03** Only one discount mechanism can be applied to an order. Loyalty points and any other discount cannot be combined.
- **BR-04** Discounts never apply to the delivery fee.
- **BR-05** Alcohol, tobacco, and gift cards are excluded from all discounts (legal requirement).
- **BR-06** Every applied discount must be shown as a separate line in the cart, at checkout, and in the order confirmation email.

## Orders

- **BR-10** Minimum order value is 15.00 EUR (before discounts, without delivery fee).
- **BR-11** Only registered customers can place an order.
- **BR-12** An order can be cancelled by the customer until it is handed to the courier.
- **BR-13** On a full or partial refund, the refunded amount is calculated from the price actually paid, after discounts.

## Loyalty

- **BR-20** A customer earns 1 point for every 1 EUR actually paid (after discounts, without delivery fee).
- **BR-21** 100 points equal a 1.00 EUR discount.

## Admin Panel and audit

- **BR-30** Any change to prices or promotions in the Admin Panel must be recorded in the audit log (who, when, what changed).
- **BR-31** Only users with the Store Manager role can create or edit promotions.

## Non-functional

- **BR-40** Cart price recalculation must respond within 500 ms for 95% of requests.
- **BR-41** All customer-facing texts must be available in English and German.
- **BR-42** Error messages must explain what went wrong and what the customer can do next.
