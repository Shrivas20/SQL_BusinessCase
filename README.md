# SQL_BusinessCase
Analysis of Sales of Retail Company to understand the learned SQL concepts

# E-commerce Data Analysis

This repository is to do a business case focused on e-commerce transactions, designed to showcase my ability to analyze and derive insights from complex datasets. Utilizing SQL and data analysis techniques, I will explore various aspects of the e-commerce platform, this project serves not only as a comprehensive application of my SQL skills but also as a key component of my professional portfolio, demonstrating my capability to solve real-world business problems through data-driven solutions.

## File Descriptions

### 1. `customers.csv`
This file contains information about the consumers who made purchases.

| Feature                      | Description                                        |
|------------------------------|----------------------------------------------------|
| `customer_id`                | ID of the consumer who made the purchase           |
| `customer_unique_id`         | Unique ID of the consumer                          |
| `customer_zip_code_prefix`   | Zip Code of consumer’s location                    |
| `customer_city`              | Name of the City from where the order is made     |
| `customer_state`             | State Code from where the order is made (e.g., SP)|

### 2. `geolocation.csv`
This file includes geographical data related to the consumers.

| Feature                      | Description                                        |
|------------------------------|----------------------------------------------------|
| `geolocation_zip_code_prefix`| First 5 digits of Zip Code                         |
| `geolocation_lat`            | Latitude                                           |
| `geolocation_lng`            | Longitude                                          |
| `geolocation_city`           | City                                              |
| `geolocation_state`          | State                                             |

### 3. `sellers.csv`
This file contains details about the sellers registered on the platform.

| Feature                      | Description                                        |
|------------------------------|----------------------------------------------------|
| `seller_id`                  | Unique ID of the seller registered                 |
| `seller_zip_code_prefix`     | Zip Code of the seller’s location                  |
| `seller_city`                | Name of the City of the seller                     |
| `seller_state`               | State Code (e.g., SP)                             |

### 4. `order_items.csv`
This file includes information about the items within each order.

| Feature                      | Description                                        |
|------------------------------|----------------------------------------------------|
| `order_id`                   | Unique ID of the order made by the consumers       |
| `order_item_id`             | Unique ID given to each item ordered               |
| `product_id`                 | Unique ID given to each product available          |
| `seller_id`                  | Unique ID of the seller registered                 |
| `shipping_limit_date`        | Date before which shipping must be completed       |
| `price`                      | Actual price of the products ordered               |
| `freight_value`              | Price rate for delivery from one point to another  |

### 5. `payments.csv`
This file contains details about the payment transactions for orders.

| Feature                      | Description                                        |
|------------------------------|----------------------------------------------------|
| `order_id`                   | Unique ID of the order made by the consumers       |
| `payment_sequential`         | Sequence of payments made (in case of EMI)         |
| `payment_type`               | Mode of payment used (e.g., Credit Card)          |
| `payment_installments`       | Number of installments in case of EMI              |
| `payment_value`              | Total amount paid for the purchase order           |

### 6. `orders.csv`
This file provides information about the orders placed.

| Feature                      | Description                                        |
|------------------------------|----------------------------------------------------|
| `order_id`                   | Unique ID of the order made by the consumers       |
| `customer_id`                | ID of the consumer who made the purchase           |
| `order_status`               | Status of the order (e.g., delivered, shipped)    |
| `order_purchase_timestamp`    | Timestamp of the purchase                          |
| `order_delivered_carrier_date`| Delivery date by the carrier                      |
| `order_delivered_customer_date`| Date customer received the product                |
| `order_estimated_delivery_date`| Estimated delivery date for the products        |

### 7. `reviews.csv`
This file includes customer reviews for the products ordered.

| Feature                      | Description                                        |
|------------------------------|----------------------------------------------------|
| `review_id`                  | ID of the review given on the product              |
| `order_id`                   | Unique ID of the order made by the consumers       |
| `review_score`               | Review score given by the customer (1-5)          |
| `review_comment_title`       | Title of the review                                |
| `review_comment_message`     | Review comments posted by the consumer             |
| `review_creation_date`       | Timestamp of when the review was created           |
| `review_answer_timestamp`    | Timestamp of when the review was answered          |

### 8. `products.csv`
This file contains details about the products available on the platform.

| Feature                      | Description                                        |
|------------------------------|----------------------------------------------------|
| `product_id`                 | Unique identifier for the product                  |
| `product_category_name`      | Name of the product category                       |
| `product_name_length`        | Length of the product name                         |
| `product_description_length` | Length of the product description                  |
| `product_photos_qty`         | Number of photos available for each product       |
| `product_weight_g`           | Weight of the products ordered (in grams)         |
| `product_length_cm`          | Length of the products ordered (in centimeters)    |
| `product_height_cm`          | Height of the products ordered (in centimeters)    |
| `product_width_cm`           | Width of the products ordered (in centimeters)     |


## Schema Diagram

![E-commerce Data](/image.png)

