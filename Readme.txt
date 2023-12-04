*Please check "main" branch for the latest changes

Task Update:

For requirement 1:
- The product page template is on Shopify 2.0 with dynamic sections, blocks and data sources
- Multiple product variants can be selected and added to the cart
- New section and blocks schema is being used
- For metafields, I have added a subtitle metafield called "product.metafields.custom.subtitle". Please look for below code in main-product.liquid
{% if product.metafields.custom.subtitle %}
    <h3>{{ product.metafields.custom.subtitle | escape }}</h3>
{% endif %}

Metafield values can be added directly in the customizer via dynamic sources or via directly in the code as I have added here.

For requirement 2:
- Product items can be added directly to the cart with a small popup allowing the users to see clearly what items have been added in the cart
- There is no page refresh

For requirement 3:
- Cart item quantities can be increased or decreased without page refresh
- Cart items can be deleted without page refresh
- A spin icon displays while these actions are in progress
- If a product reaches its max limit while increasing the quantity, a small message will be displayed right below the quantity selector to let users know that they can reached the max limit.
