Diffusion through Permutation:
    -The flow of encryption is -->Shift Rows-->Mix column-->
    -So to decrypt it -->inv_mix_column-->inv_shift_rows-->
    - s[0][1], s[1][1], s[2][1], s[3][1] = s[1][1], s[2][1], s[3][1], s[0][1]
    s[0][2], s[1][2], s[2][2], s[3][2] = s[2][2], s[3][2], s[0][2], s[1][2]
    s[0][3], s[1][3], s[2][3], s[3][3] = s[3][3], s[0][3], s[1][3], s[2][3]
    -This is the shift rows code given
    -s[0][1], s[1][1], s[2][1], s[3][1] = s[3][1], s[0][1], s[1][1], s[2][1] 
    s[0][2], s[1][2], s[2][2], s[3][2] = s[2][2], s[3][2], s[0][2], s[1][2]
    s[0][3], s[1][3], s[2][3], s[3][3] = s[1][3], s[2][3], s[3][3], s[0][3]
    -So this is the inv_shift_rows code for the decryption
    -After the decrypyion we pass the array to matrix2bytes and then decode it for  flag