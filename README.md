# Marquee Products Section for Shopify

This is a custom Shopify section that displays products in a horizontally scrolling marquee format. It supports:

- Dynamically loaded prices via FakeStoreAPI
- Image placeholder if image is missing
- Responsive layout with animation pause on hover

## Preview
Live Preview: https://marquee-products.myshopify.com/
password: yawngu

## Notes
- Price data is loaded dynamically from https://fakestoreapi.com/
- Products without a price show "Price unavailable"
- Layout is fully responsive


This section displays product cards that are fully manageable through the Shopify Customizer. Each card can be added individually, with image, title, and description set via the Customizer interface.

The product price is dynamically fetched using a fetch request from an external API (FakeStoreAPI), based on the product ID specified in the settings.

To achieve seamless infinite scrolling, all product cards are duplicated in JavaScript after prices are loaded.

A custom SVG placeholder is used as a fallback in case no image is uploaded, ensuring the layout remains consistent.

The section is reusable and functions correctly when used multiple times on the same page. No data conflicts or overwrites occur between instances.
