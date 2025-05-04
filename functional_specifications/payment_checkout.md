## Payment Processing & Checkout

- Accepted Methods:
  - Visa
  - Mastercard
    - Condition: Mastercard payments are accepted only if the total order value is $100.00 or greater. The checkout process must dynamically enable or disable the Mastercard payment option based on the cart total reaching this threshold. Orders below $100 cannot be completed using Mastercard.
  - American Express (Amex)
    - Condition: American Express payments are accepted only if the total order value (including any potential taxes or shipping fees) is $500.00 or greater. The checkout process must dynamically enable or disable the Amex payment option based on the cart total reaching this threshold. Orders below $500 cannot be completed using Amex.
- Checkout Flow: Standard e-commerce checkout process including cart review, shipping information (for B2B delivery locations), billing information, payment method selection (with conditional payment availability based on rules), and order confirmation.