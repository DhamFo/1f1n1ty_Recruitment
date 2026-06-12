Legendre Symbol:

    -(a/p) is the symbol of legendre , conditions:
        a**((p-1)/2) = 1 mod p --> Quadratic Residues
        a**((p-1)/2) = -1 mod p --> Non-Quadratic Residues
        a**((p-1)/2) = 0 mod p --> 0

    -Python logic:
        def math_1(a,p):
            return pow(r,(p-1)//2,p)
        def pow_1(a,p):
            return pow(r,(p+1)//4,p)
    
        for r in ints:
            res = math_1(r,p) --> this step gives us the number to be chk for QR

            if res == 1:      --> condition for QR
                n1 = pow_1(r,p)  --> square root of the QR since it follows p = 3 mod 4
                n2 = p-n1

        print(max(n1,n2))