### Creating SQL table with ChatGPT
This table is for beginner learners. First I am going to create simple table and after I will make it more complicated, so that it helps me to develop my skills.

**STEPS**

1. We create 3 type of tables which are Customer info, banking products, bank transactions.
   
 For the first table, use this prompt:

 "I need to create SQL tables. There will be 3 tables in total. Please create them considering the primary and foreign keys. The first table will contain 50 rows and is called Customer Info. It should include the following fields: customer_name, customer_surname, customer_age, gender, CIF_number (7 digits), identification_number (e.g., AA9086372), phone_number (e.g., +994 .. ... .. .. – can be null), address_1, and address_2 (addresses can be null). All other fields must not be null. Note: the null values should be applied randomly — some rows should contain data, while others can be null. 
 Give me row and clean data. it is for the beginners"


After getting row data from ChatGPT, go to [SQL Lite Online](https://sqliteonline.com/), first add the **Table** and click the run button, then add **Values** and click the run. 

As shown image, there should not be any error (in the right you can see SYNTAX & History section)

<img width="1655" height="631" alt="image" src="https://github.com/user-attachments/assets/b64c27f3-21a8-4e30-a55a-a92476842e81" />

 
