#### **Creating SQL table with ChatGPT**
This table is for beginner learners. First I am going to create simple table and after I will make it more complicated, so that it helps me to develop my skills.

## **STEPS**

1. We create 3 type of tables which are Customer info, banking products, bank transactions.
   
 - For the first table, use this prompt:

 "I need to create SQL tables. There will be 3 tables in total. Please create them considering the primary and foreign keys. The first table will contain 50 rows and is called Customer Info. It should include the following fields: customer_name, customer_surname, customer_age, gender, CIF_number (7 digits), identification_number (e.g., AA9086372), phone_number (e.g., +994 .. ... .. .. – can be null), address_1, and address_2 (addresses can be null). All other fields must not be null. Note: the null values should be applied randomly — some rows should contain data, while others can be null. 
 Give me row and clean data. it is for the beginners"


After getting row data from ChatGPT, go to [SQL Lite Online](https://sqliteonline.com/), first add the **Table** and click the run button, then add **Values** and click the run. 

As shown image, there should not be any error (in the right you can see SYNTAX & History section)

<img width="1655" height="631" alt="image" src="https://github.com/user-attachments/assets/b64c27f3-21a8-4e30-a55a-a92476842e81" />


  - For the second table, use this prompt:

"The name of the second table will be Bank Account.
In your opinion, which fields should be included in this table to ensure it aligns properly with the third table, Bank Transaction? "

**then** 

"give me **literal VALUES (...)** for each customer for customer_info table. Some of the **closed_at** values should not be null. Increase the number of accounts with status = "closed" to 15.
The **opened_at** dates should not all be the same — only 10 accounts should have the same opening date, while the rest should all have different dates.
Similarly, for 7 customers, the **savings** amounts should be 5-digit numbers.
Add a total of 17 accounts with currencies EUR and USD, and make sure some of them belong to accounts with status set to "closed" and account_type set to "savings".
As for the **branch_code**, 15 accounts should have the same code, while the rest should have different ones. The branch_code values should not be sequential."

After getting row data from ChatGPT, go to SQL Lite Online and add both table script and Values like the first one (like customer_info table). 

- For the last table, use this prompt:

"Create bank_transaction table. Please generate **Values** at least 5–6 transactions for each customer, ensuring they are different from each other. The amount field should represent positive values as credit and negative values as debit. The reference field should contain the idempotency key from the source system. The direction field should be either 'C' for credit or 'D' for debit. The counterparty_account field should not be null. The channel field should include values like 'POS', 'ATM', or 'Online'. The status field should support values such as 'posted', 'pending', or 'reversed'. It is required that the transactions of each customer are mixed throughout the table.
For example, transactions belonging to customer with account_id = 1 should appear at different positions — one might be on row 15, another on row 203, and so on — rather than being grouped together."

After getting row data from ChatGPT, go to SQL Lite Online and add both table script and Values like the others.

And here you are, you have data for practice. 

2. Next I will ask Chatgpt to give me tasks easy to hard and I will try to solve myself, then ask ChatGPT again whether it is correct or not.


















  
