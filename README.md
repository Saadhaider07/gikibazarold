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
