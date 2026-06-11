Modulus Inutilis:
    -In this challenge gcd(e,phi) > 1 so it doen't have modulus inverse so we cannot find d.
    -Alternate to that if we find e-th root of the cipher we can able to crack the challenge
    -def get_eth_root(c, e, n):
    low = 0
    for k in range(100):
        target = c + k * n
        low = 0
        high = target
        while low < high:
            mid = (low + high) // 2
            if mid**e < target:
                low = mid + 1
            else:
                high = mid
        if low**e == target:
            return low
    return None
    -This is the logic we written for e-th root of the cipher