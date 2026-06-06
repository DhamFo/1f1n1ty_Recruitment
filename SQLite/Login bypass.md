Vulnerability in login:
    -This challenge is done by sql injection in username and password in login page
    -The SQL for this is SELECT * FROM users WHERE username = 'wiener' AND password = 'bluecheese'
    -In this, We use "--" in the end of the username to comment the password section
    -SELECT * FROM users WHERE username = 'administrator'--' AND password = 'xyz'
    -Which comments after the username and logedin to the website  