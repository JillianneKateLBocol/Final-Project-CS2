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

LOAD order_records
choice = 0

WHILE choice != 6:
    OUTPUT "[1] Show total orders and total revenue"
    OUTPUT "[2] Show best-selling product"
    OUTPUT "[3] Show top 3 customers"
    OUTPUT "[4] Show number of orders by status"
    OUTPUT "[5] Search sales of a product"
    OUTPUT "[6] End program"
    
    OUTPUT "Choose a feature: "
    INPUT choice
    
    IF choice == 1:
        total_orders  = 0
        total_revenue = 0
        
        FOR order IN orders_list:
            total_orders  += 1
            total_revenue += total_amount
        
        OUTPUT "Total orders: ", total_orders
        OUTPUT "Total revenue: ", total_revenue

    ELIF choice == 2:
        best_selling = MAX(quantity)
        OUTPUT "Best selling product: ", best_selling

    ELIF choice == 3:
        GROUP orders BY customer
        SORT groups BY total_amount DESC
        SELECT top 3 customers
        
        OUTPUT "Top 3 customers:"
        OUTPUT "  #1: ", top_1
        OUTPUT "  #2: ", top_2
        OUTPUT "  #3: ", top_3

    ELIF choice == 4:
        GROUP orders BY status
        COUNT pending
        COUNT shipped
        COUNT delivered

        OUTPUT "Pending: ", pending
        OUTPUT "Shipped: ", shipped
        OUTPUT "Delivered: ", delivered

    ELIF choice == 5:
        OUTPUT "Search a product for its sales: "
        INPUT product
        
        SEARCH product IN orders_list
        COUNT quantity
        
        OUTPUT product, " sales: ", quantity

    ELIF choice == 6:
        OUTPUT "Exiting program. Thank you!"

    ELSE:
        OUTPUT "Invalid choice. Please try again."

END


🪢 Flowchart:
<img width="2048" height="1275" alt="591409443_1157440009831869_3451440952534326949_n" src="https://github.com/user-attachments/assets/8efdebcd-5cfb-4e6a-bafe-13655470d8a6" />
