Endles Emails:

    -In this chllenge we use Chinese remiander thrm to find plaintxt
    -Since e = 3 we need 3 combinations of N and C out of 7 given N and C
    -We use itertools library to find the possible combinations and then pass them to Chinese remainder thrm fun we use gympy2 for 3rd root to find the plain txt and decode them.

    def chinese_remainder(n, a):
    Sum = 0
    prod = 1
    for ni in n:
        prod *= ni
    for ni, a_ in zip(n, a):
        p = prod // ni
        sum_val += ai * inverse(p, ni) * p
    return sum_val % prod

