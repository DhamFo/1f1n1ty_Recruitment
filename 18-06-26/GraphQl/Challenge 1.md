Accessing private GraphQL posts:

    -GraphQL is a query language for APIs .It allows you to request exactly what you need.
    -In this challenge we use burp suite for the password
    -Once the request with the end point send to reapeter we use GeraphQL option to see the json part
    -In that we have a field of postPassword in name of Blogpost 
    -From Http history , the request again sent to repeter now in GQL tab variable panel we change the id to 3 and in query panel we introduce postPassword field and send the request and collect the password 