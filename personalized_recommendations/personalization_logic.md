# Personalization Logic

This document outlines the logic used to generate personalized banana recommendations for users on the BananaBonanza.com homepage.

## Data Sources

The following data sources are used to personalize recommendations:

*   **Past Purchase History:**  A record of all previous banana purchases made by the user.
*   **Browsing History:**  A log of the bananas the user has recently viewed or added to their wishlist.
*   **Monkey Clan Affiliations:**  The user's assigned Monkey Clan, which indicates potential banana preferences based on clan trends.

## Recommendation Algorithms

The following algorithms are used to generate recommendations:

1.  **Collaborative Filtering:**
    *   **Purchase-Based:** Identifies bananas frequently purchased by users with similar purchase histories.
    *   **Browsing-Based:** Recommends bananas frequently viewed or wishlisted by users with similar browsing histories.
2.  **Content-Based Filtering:**
    *   Recommends bananas similar to those the user has previously purchased or viewed, based on attributes like:
        *   Banana Type (e.g., Cavendish, Plantain, Red Banana)
        *   Brand
        *   Ripeness Level
3.  **Clan-Based Recommendations:**
    *   Recommends bananas that are popular within the user's Monkey Clan.

## Fallback Recommendations

For new users with no purchase or browsing history, the system will display:

*   **Popular Bananas:**  The most popular bananas across the entire BananaBonanza.com platform.
*   **Prompt for Personalization:** A message suggesting they create an account or browse the catalog to receive personalized recommendations.

## Algorithm Weighting

The system will dynamically adjust the weighting of each algorithm based on:

*   **Data Availability:**  If a user has limited purchase history, browsing-based and clan-based recommendations will be weighted more heavily.
*   **Performance Metrics:**  The system will continuously monitor the performance of each algorithm (e.g., click-through rate, conversion rate) and adjust the weights accordingly to optimize recommendations.