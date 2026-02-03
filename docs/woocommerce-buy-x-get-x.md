# How to Set Up WooCommerce Buy One Get One Free (Buy X Get X)

Boost your store's average order value with compelling "Buy X Get X" offers. **YeeDiscounts** makes it easy to create powerful BOGO promotions where customers get the *same* product as a reward (e.g., Buy 1 T-Shirt, Get 1 T-Shirt Free).

## 1. Creating a New Rule
1. Navigate to **WooCommerce > Settings > Dynamic Discounts**.
2. Click **Add New Rule**.
3. Enter a **Rule Name** (e.g., "T-Shirt BOGO Special").
4. (Optional) Set a unique **Rule ID** or let it generate automatically.

## 2. Configuring the Discount
In the **Discount Type** section, select:
*   **Discount Type**: `Buy X Get X (Same Product)`

This mode is designed for offers where the customer buys a specific quantity of a product and gets a reward quantity of the *same* product.

### Setting Up Tiers (Ranges)
The plugin uses a flexible "Tier" system to define your Buy/Get logic.

1.  Click **Add Range** to create your first tier.
2.  **Min Qty**: The number of items the customer must buy to trigger the deal (e.g., `1` for Buy 1 Get 1).
3.  **Discount Type**:
    *   **Free**: The reward item is 100% free.
    *   **Percentage**: The reward item is discounted by a percentage (e.g., Buy 1, Get 2nd at 50% off).
    *   **Fixed Amount**: The reward item is discounted by a fixed dollar amount.
4.  **Value**:
    *   If configuring a **Percentage** or **Fixed Amount**, enter the value here (e.g., `50` for 50% off).
    *   If **Free**, this value is ignored (automatically 100%).
5.  **Recursive (Repeat)**:
    *   Check this box if you want the rule to repeat for every multiple of the Min Qty.
    *   *Example*: With Min Qty 1 and Recursive enabled:
        *   Buy 1, Get 1 Free.
        *   Buy 2, Get 2 Free.
        *   Buy 10, Get 10 Free.

## 3. Filtering Logic (Who gets the deal?)
Use the **Filter** section to determine which products qualify for this BOGO offer.

*   **Filter Type**:
    *   **Specific Products**: Select specific items (e.g., "Logo T-Shirt").
    *   **Product Categories**: Apply to entire categories (e.g., "Hoodies").
    *   **All Products**: Apply store-wide.
*   **Operator**: `In List` (Include) or `Not In List` (Exclude).

## 4. Common Examples

### Scenario A: Buy 1 T-Shirt with Logo, Get 1 Free
*   **Discount Type**: Buy X Get X
*   **Filter**: Select specific product "T-Shirt with Logo" (Filter Type: Products, Operator: In list).
*   **Min Qty**: `1`
*   **Recursive**: `Checked` (Yes)
*   **Tier Type**: `Free`
*   **Result**: When a customer adds **1** "T-Shirt with Logo" to their cart, the plugin automatically adds another **1** "T-Shirt with Logo" for free. They pay for 1, they get 2.

<img src="https://add-ons.org/wp-content/uploads/2026/02/WooCommerce-set-up-buy-1-get-1-1024x697.png" alt="Setting Buy 1 get 1" class="aligncenter size-large" style="max-width: 100%; height: auto;" />
<p style="text-align: center;">Setting backend</p>

<img src="https://add-ons.org/wp-content/uploads/2026/02/Cart-buy-1-get-1-1024x464.png" alt="Cart page" class="aligncenter size-large" style="max-width: 100%; height: auto;" />
<p style="text-align: center;">Cart page</p>

## 5. Saving the Rule
Once configured, scroll to the top or bottom and click **Save Rule**.

---
*Note: Ensure your "Show on-sale badge" settings are configured in the active rule or global settings if you want to highlight these products in the shop.*
