
# Conceptual business model: A board game store

This model is for a boardgames store, and this store can be physical or an e-commerce

## Part 1: Conceptual business model

Construct a conceptual business model for an industry or business that you are familiar with or have interest in

•	Your model should represent at least 10 ideas

•	It should visually represent one to one, many to one, or many to many relationships among ideas


 ![image](https://user-images.githubusercontent.com/71708626/96743060-fa962500-1399-11eb-8ab9-33a4ea2aed01.png)



## Part 2: Relational data model

Take a subset of the ideas from the conceptual model you constructed in Part 1 and design a simple relationship model. 


•	Your model should have at least 5 tables

•	You should include at least 20 attributes, or fields, in your model (20 total across all tables, not per table)

•	Your model should be normalized

•	Identify the primary key in each table, and state whether it is a natural or surrogate key

•	For each relationship between tables, identify any foreign keys needed to define the relationship

•	For each table, identify what type of system or systems you think the data might come from.

![image](https://user-images.githubusercontent.com/71708626/96746815-f2d87f80-139d-11eb-9416-24f0309eb479.png)

![image](https://user-images.githubusercontent.com/71708626/96743187-1994b700-139a-11eb-8b7d-2cdd3beb9959.png)
 
## Part 3: SQL queries

Using the data model you constructed in Part 2, come up with two data extracts you think would be interesting, then write SQL queries to provide each one.

•	For each query, state what data you are trying to get and why it would be interesting

•	Provide the SQL query using the commands and syntax we learned in Module 3

•	For maximum credit, at least one of your queries should involve a join across two or more tables.

**Code 1: which game publisher sells best**

Each board game is developed by a company (publisher). Each publisher produces several games, in the most varied categories and prices. Many players have a preference for certain publishers, as each brings different mechanics, quality of components, etc.
So it is important to know which publisher sells best to know which one is more advantageous to form a partnership to develop events and promotions for customers aiming at their loyalty and also increase sales

![image](https://user-images.githubusercontent.com/71708626/96746537-a8ef9980-139d-11eb-98b7-6bcb1e8226f2.png)

**Code 2: Most game is sold for each type of mechanics**

In the world of board games there are different types of strategy (reasoning, luck or both) and different types of mechanics (deck bulding, card drafting area control, workers allocation, rolling dice, etc.). In general, players prefer certain types of mechanics.
So it is important to know which of these games has the most output, so a promotional campaign can be more targeted to the customer's taste.

![image](https://user-images.githubusercontent.com/71708626/96746446-8f4e5200-139d-11eb-8397-50d53acf9706.png)


## Part 4: Sensitive data and data quality issues

Consider the data privacy and data quality implications of the data model you constructed in Part 2.

•	Identify any fields you think might be PII, CFI, CPNI, or PHI.

•	What data elements in your model will present the most significant data quality challenges? Explain your reasoning.

1- In the second part, the tables related to the product as characteristics and suppliers were presented. Thus, the most sensitive data would be related to the purchase of the product (CFI), such as the price the publisher sells the games for, or even how much it buys some titles from abroad, etc. Beyond that point, but not shown in the tables, it would be in relation to customer data (PII), such as the CPF (which in Brazil equals social insurance), email and address.

2- Among the various steps that can generate problems in data quality, the most important are in relation to customer registration, games registration and receipts. The registration of customers is often carried out online, that is, they will not always perform them correctly or may not even complete all fields. Which can generate invoices with errors or even problems in product delivery. As board games have many characteristics and there may be some error when cataloging all games, which can cause some problems when making an announcement in the online store or even errors in data analysis to create specific promotions as mentioned in step 3. In Brazil, when we sell a product, we have to issue notes from those sales, which can be used as legal evidence, as making sure these notes are correct is very important. In addition, it is through the data in these notes that companies make some bludgers.



