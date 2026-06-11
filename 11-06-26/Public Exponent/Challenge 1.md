Salty:
    -In this we have e = 1 (small).This leads to fast encryption and verfication
    -The given n is prime number so phi = n-1
    -The private key is d = inverse(e,phi)
    -The decryption is pt = pow(ct,d,n)