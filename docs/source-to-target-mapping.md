# Source-to-Target Mapping

## 1. dim_customer

### Source
olist_customers_dataset.csv

### Grain
One row represents one customer record.

### Mapping

| Target Column | Source Column | Transformation |
|---|---|---|
| customer_key | N/A | Generate surrogate key |
| customer_id | customer_id | Direct |
| customer_unique_id | customer_unique_id | Direct |
| zip_code_prefix | customer_zip_code_prefix | Rename |
| city | customer_city | Standardize |
| state | customer_state | Standardize |
| effective_start_date | N/A | Pipeline date |
| effective_end_date | N/A | 9999-12-31 |
| is_current | N/A | TRUE |

## 2. dim_product

...

## 3. dim_seller

...

## 4. dim_date

...

## 5. fact_sales

...

## 6. fact_payment

...

## 7. fact_review

...