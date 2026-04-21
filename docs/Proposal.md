📌 Project Proposal (Final)
📝 Eccomerce Analyzer
-- Eccomerce.JSON

🔍 Problem Statement: 

Many online stores struggle with efficiently managing orders and products, which creates challenges for both businesses and customers. Poor inventory tracking often leads to overselling or stockouts, while delayed order processing results in customer dissatisfaction. These issues not only harm customer trust but also limit the store’s ability to scale and compete in the fast-paced e-commerce industry. Developing effective solutions for order and product management is therefore crucial to improving customer experience and ensuring business growth.


🎯 Project Objectives:

Objective 1: To analyze and summarize key information from the ecommerce dataset, including sales trends, top-selling products, and customer purchasing behavior.
Objective 2: To help users gain meaningful insights. These include seasonal demand, popular categories, and average spending that can support better decision-making in ecommerce businesses.
Objective 3: To practice JSON handling, Python programming, and data analysis techniques by working with real-world ecommerce data.

⚙️ Planned Features:

Feature 1 (Starter Idea): Show total orders and total revenue
Feature 2 (Starter Idea): Show best-selling product
Feature 3: Show top 3 customers
Feature 4: Show number of orders by status
Feature 5: Search sales of a product

⌨️ Planned Inputs and Outputs:

Inputs:
; Order ID, customer name, order date, status, payment method, home address, items, product.

Outputs:
; Category, price, quantity, total amount.

🧠 Logic Plan:
This section showchases the flowchart and pseudocode of the proposal.

🫀 Pseudocode:

START
  DECLARE choice, total_orders, total_revenue : INTEGER
  DECLARE best_selling, quantity, product : STRING
  DECLARE top_1, top_2, top_3, status, pending, shipped, delivered : STRING

  LOAD order_records FROM database

  WHILE TRUE DO
    DISPLAY "[1] Show total orders and total revenue"
    DISPLAY "[2] Show best-selling product"
    DISPLAY "[3] Show top 3 customers"
    DISPLAY "[4] Show number of orders by status"
    DISPLAY "[5] Search sales of a product"
    DISPLAY "[6] End program"
    
    INPUT choice
    
    IF choice = 1 THEN
      CALL Process_A(order_records)
    ELSE IF choice = 2 THEN
      CALL Process_B(order_records)
    ELSE IF choice = 3 THEN
      CALL Process_C(order_records)
    ELSE IF choice = 4 THEN
      CALL Process_D(order_records)
    ELSE IF choice = 5 THEN
      CALL Process_E(order_records)
    ELSE IF choice = 6 THEN
      CALL Process_F(order_records)
      BREAK loop
    ELSE
      DISPLAY "Invalid choice. Please try again."
    END IF
  END WHILE
END

FUNCTION Process_A(order_records):
  total_orders = 0
  total_revenue = 0
  FOR EACH order IN order_list DO
    total_orders = total_orders += 1
    total_revenue = total_revenue += total_amount
  END FOR
  DISPLAY "Total orders: ", total_orders
  DISPLAY "Total revenue: ", total_revenue
RETURN

FUNCTION Process_B(order_records):
  best_selling = MAX(quantity)
  DISPLAY "Best-selling product: ", best_selling
RETURN

FUNCTION Process_C(order_records):
  Group orders by customer
  Sort in descending based off total_amount
  Select top 3 customers (top_1, top_2, top_3)
  DISPLAY "Top 3 customers: "
  DISPLAY "#1: ", top_1
  DISPLAY "#2: ", top_2
  DISPLAY "#3: ", top_3
RETURN

FUNCTION Process_D(order_records):
  Group orders by status
  Count pending
  Count shipped
  Count delivered
  DISPLAY "Pending: ", pending
  DISPLAY "Shipped: ", shipped
  DISPLAY "Delivered: ", delivered
RETURN

FUNCTION Process_E(order_records):
  DISPLAY "Search a product for its sales: "
  INPUT product
  Search product in list
  Count quantity
  DISPLAY product, "sales: ", quantity
RETURN

FUNCTION Process_F(order_records):
  CLOSE database connection
  DISPLAY "Exiting program. Thank you!"
RETURN

🪢 Flowchart:
<img width="2048" height="1275" alt="591409443_1157440009831869_3451440952534326949_n" src="https://github.com/user-attachments/assets/8efdebcd-5cfb-4e6a-bafe-13655470d8a6" />
