File path traversal, traversal sequences stripped with superfluous URL-decode:

    -Web servers may strip the sequence traversal and decode the url for checking before sending to the application
    -So , for that we use double encoding. Even if it does one layer decoding it will not find the traversal sequence and bypass it 
    -https://0a84006e04181beb81f2110700ad0062.web-security-academy.net/image?filename=%252e%252e%252f%252e%252e%252f%252e%252e%252f/etc/passwd