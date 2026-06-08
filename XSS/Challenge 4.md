DOM XSS in innerHTML sink using source location.search:
    -In this we need to write the script on the search bar
    -A random string is written in the search bar.After the result in the inspection tab found a javascript code
    -There .innerHTML = query
    -The innerHTML will not accept script or svg onload. So insted of this we use img or iframe we can use onerror key word
    -So <img src=1 onerror=alert()> is the code we wrote in search bar