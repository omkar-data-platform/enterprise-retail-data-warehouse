# Retail Data Warehouse - Data Model

## Source Tables

1. customers
2. orders
3. order_items
4. order_payments
5. order_reviews
6. products
7. sellers
8. geolocation
9. product_category_translation

## Fact Tables

### fact_sales
Grain:
One product item within an order.

### fact_payment
Grain:
One payment record associated with an order.

### fact_review
Grain:
One review record associated with an order.

## Dimension Tables

### dim_customer
### dim_product
### dim_seller
### dim_date
### dim_geography