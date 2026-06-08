DOM XSS in document.write sink using source location.search:
    -We write some string in the search bar and inspect the page where the string is placed.
    -The string is found in a src of image tag.
    -So we do "><svg onload=alert(1)>.
    -When the javascript finds <svg> it immediately excute this code