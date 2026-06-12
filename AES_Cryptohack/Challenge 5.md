Confusion through Substitution:

	-The main motive of this is  inverse sub box
	-The mapping of the sbox is Galois Field GF(2**8) 
	-So to inverse the sbox we need to use
	-cur = s[i][j]
	 s[i][j]=inv_s_box[cur]
	-Then append this to txt and convert to bytes and decode them.
