Stored cross-site scripting:
    -We need to perform a cross-site scripting that calls alert() function in the comment section of the post
    -In comment section  type <script>alert()</script>
    -Any user who visit the post will now recerive <p><script>alert()</script></p>
    -Then it will be excuted in the users browser