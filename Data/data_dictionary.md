📑Example Datasets
✔ Orders dataset
Provide information about orders

order_id: unique ID of the order
customer_id: unique ID of the customer
order_status: order status
order_purchase_timestamp: time when the order was ordered
order_approved_at: time the order is approved
order_delivered_carrier_date: the time the item was delivered to the carrier
order_delivered_customer_date: the time the item was delivered to the customer
order_estimated_delivery_date: the estimated time the order will be delivered to the customer

✔ Order items dataset
Provide information about each item in the order and shipping costs

order_id: unique ID of the order
order_item_id: ID of the item in the order (item number 1 has ID 1, item 2 has ID 2, etc. Based on this we also know how many items each order has)
product_id: unique ID of the product in the order
seller_id: unique ID of the seller
price: the price of the item
freight_value: shipping fee

✔ Order payments dataset
Provide information of order payments.

Note that we need to combine all values of each order to have total values.

order_id: unique ID of order
payment_sequential: sequence order
payment_type: payment type
payment_installments: full payment (payment_installments = 1) or installment (payment_installments > 1),total payment is splited to many payments .
payment_value: payment value (payment_value - equal total payments of all times payment installments)

✔ Product dataset
Provide product information

product_id: unique ID of product
product_category_name: category product name
product_name_lenght: number of product name letters
product_description_lenght: number of product description letters
product_photos_qty: number of product photo
product_weight_g: weight of product (g)
product_length_cm: length of product (cm)
product_height_cm: height of product (cm)
product_width_cm: width/deep of product (cm)

✔ Order reviews dataset
Provide review details of each order

review_id: unique ID of revie
order_id: unique ID of order
review_score: Review Score
review_comment_title: Comment title
review_comment_message: detail of review
review_creation_date: Created date of review
review_answer_timestamp: timestamp of review answers
Click to expand Order Reviews Dataset

✔ Customers dataset
Provide Customer Information

customer_id: customer unique ID used to link with customer_id of orders_dataset table.
customer_unique_id: mã unique ID of customer in system of customer information management.
customer_zip_code_prefix: zip code of customer
customer_city: City name of customer
customer_state: State name of customer
