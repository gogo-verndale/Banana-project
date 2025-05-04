# Improve Banana Quantity Selection in Checkout

## Story Details
*   **Story ID:** MONKEY-124
*   **Story Title:** Improve Banana Quantity Selection in Checkout
*   **Story Type:** Improvement
*   **Priority:** Medium
*   **Story Points:** 3

## User Story
*   **As a:** Lazy Monkey Customer
*   **I want to:** Be able to easily increase or decrease the quantity of bananas in my cart using dedicated buttons within the checkout page
*   **So that:** I can quickly adjust my order without having to manually type in the desired quantity.

## Description
Currently, monkeys can only change banana quantities in the cart by manually typing a number into a text field. This is clunky and annoying, especially when they only need to add or remove a small amount of bananas. This story will add "+" and "-" buttons next to the quantity field to allow for quick and easy adjustments.

## Acceptance Criteria
*   **Given:** A Monkey Customer is viewing the checkout page with bananas already added to their cart.
    *   **When:** The Monkey Customer views the banana quantity for each item in the cart.
    *   **Then:** Each banana item's quantity field displays "+" and "-" buttons directly adjacent to it.

*   **Given:** A Monkey Customer clicks the "+" button next to a banana item's quantity.
    *   **Then:** The quantity for that item is increased by 1.
    *   **And:** The cart total is automatically updated to reflect the change.

*   **Given:** A Monkey Customer clicks the "-" button next to a banana item's quantity.
    *   **Then:** The quantity for that item is decreased by 1.
    *   **And:** The cart total is automatically updated to reflect the change.

*   **Given:** A Monkey Customer has only one of a particular type of banana in their cart and clicks the "-" button.
    *   **Then:** The item's quantity decreases to 0.
    *   **And:** The item is removed from the cart.
    *   **And:** A confirmation message should appear "Are you sure you want to remove this item?" with option to confirm and a cancel option to re-add the product to the basket.

## Additional Considerations
*   **Usability:** The "+" and "-" buttons should be clearly visible, easily clickable, and appropriately sized for monkey fingers.
*   **Mobile Responsiveness:** The buttons should function correctly and maintain visual appeal on all screen sizes (desktop, tablet, mobile).