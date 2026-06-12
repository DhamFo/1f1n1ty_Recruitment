Successive Powers:

    -Given a list of integers ,the given integers are the remainder of large succesive powers of x modulo p(three digit)
    -x^k,x^(k+1),.... mod p , then x = r1.p + a1 , x = r2.p + a2 ,....
    -Relation is x = (a2/a1) mod p general formula is x = (a[i+1]/a[i]) mod p  ,i = 1,2,3..
    => a[i]*r - a[i+1] = K.p  where r is from 1-1000
    -By this logic ,coded in python to get the p,x for this level 
