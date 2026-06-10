Manyprime:
    -In this challenge we have upto 30 factors for n 
    -So phi(n)=(P1-1)*(P2-1)*...(Pk-1)
    -For that we use for loop to multiply
    for r in range(0,len(prime),2):
        phi=phi*(prime[r]-1)*(prime[r+1]-1)
    -Rest of all is same