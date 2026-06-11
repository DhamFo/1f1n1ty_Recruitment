File path traversal, simple case:
    -This topic explore us how to change the driectory of the webpage to get required things
    -<img src="/loadImage?filename=218.png"> this image is stored in the /var/www/images/ .So the image will be in /var/www/images/218.png path 
    -This challenge consist of path traversal via url of an image to password section
    -https://0a8b00d50306c93c80f6c1c100ea00f0.web-security-academy.net/image?filename=../../../etc/passwd
    -We use ../../../ to move up to the driectory.