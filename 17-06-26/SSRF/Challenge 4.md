SSRF with blacklist-based input filter:

    -In this challenge we bypass the request by encoding
    -The request http://127.1/admin is blocked request because /admin is considered as bad parameter
    -So we double-encode the letter 'a' to bypass the security