Basic SSRF against the local server:

    -This challenge is basic SSRF attack against server
    -Application make an HTTP request back to the server that is hosting the application
    -Here we change the stockAPI parameter to http://localhost/admin/delete?username=carlos
    -The application normally will not show content in /admin but the administrative functionality is normally only accessible to authenticated users , the localhost will bypass this drawback
    