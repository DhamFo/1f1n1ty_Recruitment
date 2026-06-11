File path traversal, validation of file extension with null byte bypass:
    -Applications will expect the correcct extention in end of the name to open it 
    -If use../../../etc/passwd it will be consider as ../../../etc/passwd.png so no such file in the driectory
    -To bypass this we used %00 which is encoded version of \0 null char which is often used in C language in the end of the string. It will terminate char after this 
    -../../../etc/passwd%00.png will be terminated after passwd.