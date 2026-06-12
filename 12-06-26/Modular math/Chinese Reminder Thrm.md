Chinese Remainder Theorem:
    -In this challenge We come to know about Chinese Remainder Theorem
        x = a1 mod m1
        x = a2 mod m2
        ..
        x = an mod mn
    -To find x ,
        M = m1*m2*...mn
        Mi = M/mi                             i=1,2,3,...n
        Yi = Mi**(-1) mod mi
        x =sum(ai*Mi*Yi) mod(M)
    -In this challenge they gave three eqn of x.  x ≡ a mod 935 find a 
    -To find a we need to find x and use that for finding a 
    -   from Crypto.Util.number import inverse
        m = [5,11,17]
        a= [2,3,5]
        y=[]
        M=1
        Mi=[]
        for r in range(len(m)):
            M=M*m[r]
        x = 0 
        for r in range(len(m)):
            Mi.append(M//m[r])
            y_1 = inverse(Mi[r],m[r])
            y.append(y_1)
            x = x+a[r]*Mi[r]*y[r]

        x=x%M
    
        print(pow(x,1,935))
 