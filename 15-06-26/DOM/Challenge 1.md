DOM XSS using web messages:

    -This challenge tells us vulnerability occurring through the improper handling of web messages
    -The application uses addEventListener() fun that listen the incoming message. The javascript takes the message insert directly on DOM page.
    -So we craft a iframe tag for this 
     <iframe src="SESSION-ID-URL" onload = "this.contentWindow.porstMessage('<img src = 1 onerror = print()>','*')" >