# Branch's Data Engineering take home project : randomuser.me API

### Introduction

This is a take home project for data engineering from Branch. The dataset being provided is from randomuser.me API.I have used 1 JSON dataset which contains 500 records randomly generated. Based on the data, I have designed 5 dimension tables and write the data for each table into csv format.

- randomuser.me API: This data comes from randomuser.me API. [This](https://randomuser.me/api/?results=500)

### Files
- ETL.ipynb the scripts I wrote for the project as well as the quality check results
- staging_table.PNG the star schema diagram screenshot used for this project
- dim_tables.PNG the star schema diagram screenshot used for this project
- README.md provides discussion on the process and decisions


#### Dimension Tables
- dim_users - user data
username, gender, title, first_name, last_name, DOB, age, registered_date, registered_age
- dim_user_address - user address data
address_id, username, street ,city ,state ,postcode ,latitude ,longitude 
- dim_user_contact - user contact data
contact_id, username, phone ,cell ,id_name ,id_value
- dim_user_picture - user picture
user_picture_id, username, picture_large, picture_medium ,picture_thumbnail
- dim_login - user login information
uuid ,username ,password ,password_salt ,password_md5 ,password_sha1 ,password_sha256 ,nat

#### How to Run
1. Execute ETL.ipynb from jupiter notebook