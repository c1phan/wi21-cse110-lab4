# Part3: Debugging using the DevTools
## DevTools - Debugging
### Break  
  
![alt text](break.png)  
### Watch  
  
From this image below, you can see that the data type of result is a string.  
  
![alt text](watch.png)
### Fix 
   
The bug is that `num1` and `num2` are both of data type string, so when they get added together it'll just append `num2` to `num1`. I fixed this problem by casting the values of `num1` and `num2` to integers using `Number()`.  
  
![alt text](fix.png)  