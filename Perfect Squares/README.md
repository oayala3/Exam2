Given a positive integer n, find the least number of perfect square numbers (for example, 1, 4, 9, 16, ...) which sum to n.    
**Solution**
What you have to do to find the lowest amount is define the base case, wich is 1. You can do this the simple way, no dynamic way by caliing the funtion recursivky with all of the square numbers  
that are less than the number N. Then selecting the one that is lthe least. The way you can solve it dynamically is, **Create an array to save answers arr[n+1]**. Then fill it up every time you  
calculate a new answer. You will subtract the square number from N. And call the function again with the new number keeping count. Then You will compare the result with thr prevoius  
one saved on the array.

**Step 3**  
I think This was a combination of both duke and IDEAl  
The fact being that this is a complicated solution made me go back and delete several times what i had because I checkde them by hand following my instructions  
It is still complucated to understand and dollow.  
I used DUKE aproach solving 3 examples by hand. Then I used Pattern recognition. I used the IDEAL step to explore.  I tried using a different logic to solve the problem.  
And also tried to see if there was a formula that could explain this better
