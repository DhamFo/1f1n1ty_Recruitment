Structure of AES:
	-They gave a python code to encrypt the txt and asked us to write the code for decrytion for given matrix
	-Code for the decryption is
	 def matrix2bytes(matrix):
    		text=[]
    		for i in range(len(matrix)):
        			for j in range(len(matrix)):
            				text.append(matrix[i][j])
   	return bytes(text)
	matrix = [[99, 114, 121, 112],[116, 111, 123, 105],[110, 109, 97, 116],[114, 105, 120, 125]]
	a=matrix2bytes(matrix)
	print(f"{a.decode()}")