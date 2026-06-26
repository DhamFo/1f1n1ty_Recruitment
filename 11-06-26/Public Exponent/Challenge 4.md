Crossed Wires:

    -Given cipertext is encrypted with their own public key  => cipher = pow(cipher, key[1], key[0]) in forloop
    -In the output txt given by the challenge, contains my private key(N,D) and frnds public key and encrypted flag
    -We first find Factors of N and used it to find phi(N) 
    -Using the public key frnds and phi value we find D value using inverse() function in for loop
    -then cipher = pow(cipher, D, N) in forloop ,find the flag