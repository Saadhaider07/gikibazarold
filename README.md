# gikiolx
A semester project for DataBase Management Systems. This is an online buy/sell app for GIK Institute.

Entity Relation Diagram:

Entities:
1) User
           Attributes:
                           -Username
                           -User id (Primary Key)
                           -Email
                           -Product ID (Foreign Key)

2) Product
           Attributes:
                           -Product Id (Primary Key)
                           -User ID (Foreign Key)
                           -Product Name
                           -Upload Date
                           -Price


Relationships:
(user <-> product)
User to product: Optional (zero-to-Many)
Product to User: Mandatory (one-to-one)

3) Figma Design
   ![image](https://github.com/Saadhaider07/gikibazar/assets/162680430/180da233-47a3-40aa-85ff-c158cad50561)

   
4) ER diagram for database with following models:
   Entities:
 Users
           Attributes:
                           -phone_number INT(Primary Key) 
                           -email VARCHAR NOT NULL, UNIQUE
                           -username VARCHAR NOT NULL, UNIQUE
                           -profile_pic BYTEA/BLOB

 Products
           Attributes:
                           -prod_id INT (Primary Key)
                           -phone_number INT (Foreign Key)
                           -prod_name VARCHAR, NOT NULL
                           -prod_description VARCHAR, NOT NULL
                           -prod_price INT, NOT NULL
                           -contact_note VARCHAR
                           -product_pic BYTEA/BLOB, NOT NULL
                           -prod_available_campus BOOLEAN NOT NULL
