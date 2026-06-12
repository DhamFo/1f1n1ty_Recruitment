Quadratic Residues:

    -Quadratic Residues mean if a**2 = x modp exist in Fp then a is said to be Quadratic Residue
    -p = 29 , a = 5 ,a**2 = 11 mod 29 means sq root of 5 is 11
    -The logic we use here is 
        for r in ints:

        for i in range(1,p):
        
            if pow(i,2,p)==r:
                
                print(min(i,p-i))