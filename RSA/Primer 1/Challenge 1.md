Factoring:

    -This challenge let us to find p and q of a given 150 bit number n
    -We use factordb module
    -from factordb.factordb import FactorDB
    number=510143758735509025530880200653196460532653147 
    f=FactorDB(number)
    f.connect()
    prime=f.get_factor_list()
    print(prime)
    -This is the python code for finding p and q
    -It connect to database and return the value
