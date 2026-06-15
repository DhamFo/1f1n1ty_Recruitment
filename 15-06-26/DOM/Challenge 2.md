DOM XSS using web messages and a JavaScript URL:

    -The application uses addEventListener() fun that listen the incoming message. The javascript takes the message insert directly on DOM page.
    -It also contains indexOf() to check the string "https:" or "http:"
    -<iframe src="SESSION-ID-URL" onload = "this.contentWindow.porstMessage('javascript:print()//https:','*')" >
    -javascript:print() --> Excutes the print function , // --> comments after this 
    
