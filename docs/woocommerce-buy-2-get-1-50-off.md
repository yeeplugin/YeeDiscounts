# How to Set Up Buy 2 Get 3rd Item 50% Off (Buy X Get X)

Create compelling volume discounts where customers are rewarded for buying more of the same product. In this guide, we'll set up a rule where purchasing **2 items** qualifies the customer to get the **3rd item at 50% off**.

## 1. Creating a New Rule
1. Navigate to **WooCommerce > Settings > Dynamic Discounts**.
2. Click **Add New Rule**.
3. Enter a **Rule Name** (e.g., "Buy 2 Get 3rd 50% Off").

## 2. Configuring the Discount
In the **Discount Type** section, select:
*   **Discount Type**: `Buy X Get X (Same Product)`

### Setting Up Tiers (Ranges)
We need to configure the rule so that for every 2 items bought (full price), the next 1 item gets 50% off.

1.  Click **Add Range**.
2.  **Min Qty**: `2`
    *   This is the "Buy X" part. The customer buys 2 units at full price.
3.  **Discount Type**: `Percentage`
    *   We want to discount the reward item, not give it for free.
4.  **Value**: `50`
    *   This applies a 50% discount to the reward item.
5.  **Recursive (Repeat)**: `Unchecked` (or `Checked`)
    *   **Unchecked**: The deal applies once per order. (Buy 2, get 3rd 50% off. Buy 6, still only 1 item is 50% off).
    *   **Checked**: The deal repeats. (Buy 2, get 1 at 50% off. Buy 4, get 2 at 50% off).
    *   *Recommendation*: Check this if you want to thank customers for bigger orders!

## 3. Filtering Logic
Select which products this deal applies to.

*   **Filter Type**: `Specific Products` (e.g., "Summer T-Shirt") or `Product Categories`.
*   **Operator**: `In List`.

## 4. Result
*   **Scenario**: Customer adds **3** "Summer T-Shirts" to the cart.
*   **Outcome**:
    *   2 Items = Full Price.
    *   1 Item = 50% Off.
    *   Total quantity in cart: 3.

---
*Note: This rule uses the "Buy X Get X (Same Product)" logic. The 50% discount is applied to the additional "Get" item(s) essentially, or more accurately, standard BOGO logic in YeeDiscounts usually treats the set as a group. Ensure you test the cart total to verify.*
