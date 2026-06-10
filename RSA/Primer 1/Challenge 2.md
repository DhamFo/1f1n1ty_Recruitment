Inferius Prime:
    -It has 160 bits n and ct.Given two files .py and .txt.
    -.py contains RSA encryption and decryption. .txt contains n,e and ct
    -Used factordb module to factorise n for p and q
    -p and q used for phi(n),it is used to calculate d
    -And the d is used to decrypt
    -#!/usr/bin/env python3

    from Crypto.Util.number import getPrime, inverse, bytes_to_long, long_to_bytes, GCD
    from factordb.factordb import FactorDB

    n=984994081290620368062168960884976209711107645166770780785733 
    f=FactorDB(n)
    f.connect()
    prime=f.get_factor_list()
    p,q=prime[0],prime[1]

    e = 0x10001
    phi = (p - 1) * (q - 1)
    d = inverse(e, phi)

    ct=948553474947320504624302879933619818331484350431616834086273

    pt = pow(ct, d, n)
    decrypted = long_to_bytes(pt)
    print(decrypted)