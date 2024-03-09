# Design
This document contains the thought process that was followed while architecting, designing and developing this project.

## Process
1. Identify the features by doing a surveying the [internet.](https://www.webalive.com.au/ecommerce-website-features/)
2. Define actors, actions and entities
3. Architect a basic model for each actor
4. Develop action flows and pathways
5. Write code for each of the features

## Goal
Create APIs to sell products to customers!

## Actors
Actors are users of our product.
Actors that involved in this buy-sell cycle are
1. Buyers - Our customers who will purchase the products.
2. Sellers - Those users who sell their products to the buyers
3. Carriers - Those users who will pick up the product from the seller and deliver it to the buyer.

## Entities
1. Products - Entities that are listed and ready to be sold.
2. Orders - Entities that are sold and are being delivered or already delivered.
3. Reviews - Entities that contain the feedback of a product by the buyers
4. Ratings - Entities that contain the ratings of a product by the buyers

## Actions
Actions are performed by actors on entities. Some defined actions are
- General User Actions -
  1. CRUD Users
  2. Authenticate and authorize (OAuth, passwordless, biometric, 2FA, Autologout)
  3. CRUD Addresses

- Seller Actions - 
  1. CRUD Product
  2. List Products w/ Pagination
  3. Revenue charts

- Carrier Actions -
  1. Pick up Order
  2. Deliver Order (FSM??)

- Buyer Actions - 
  1. Product details, Related products, Featured/Recommended products
  2. Product Search w/ Pagination, Tags and Filters
     1. Filter type
        1. Category (clothing, electronics etc)
        2. Brand
        3. Price Range
        4. In stock
        5. Ratings
  3. Add, Remove and List items in cart
  4. Prebook, Place, List, Cancel, Track Order, Return
  5. CRUD Reviews and Ratings
  6. Share products
  7. Add, remove and view Wishlist

## Future Ideas
1.  **Product Videos**: Videos highlighting product features to increase conversions.
2.  **FAQ For Products**: Addresses common pre-sales questions about products.
3.  **FAQ For The Store**: Answers general questions about the store's policies.
4.  **Email Opt-In**: Encourages visitors to subscribe for future sales and promotions.
5.  **Push Notifications**: Keeps visitors updated with promotions via browser notifications.
6.  **Chatbots**: Provides support to customers 24/7 with automated assistance.
7.  **Coupon Codes**: Offers discounts to keep customers engaged during checkout.
8. **Gift Registries**: Drives sales by providing registries for special occasions.
9. **Loyalty Program**: Encourages customer retention with rewards for purchases.
10. Ads, Promotions and New Releases

## Local Development Considerations
To make development easier, I have used [fakestoreapi](https://fakestoreapi.com/) data in my fixtures.