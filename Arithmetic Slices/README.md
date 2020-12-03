A sequence of number is called arithmetic if it consists of at least three elements and if the difference between any two consecutive elements is the same.
So this problem means that the numbers have to be going up by a sum or a subtration of the same amount. 1 (plus 2) 3 (plus 2) 5  
To count i has to be 3 or more numbers.  
**Solution**  
To solve this you can do a simple solution wich would be, check the difference between arr[i] and arr[i+1], then compare that to arr[i+1] and arr[i+2]. If it is the same
If it is do arr[i+2]=arr[i+1]+1
If it is not arr[i+2]=0
**PART2**  
create an array of the same leght.  

**PART3**  
The steps Of IDEAL are
Identiy- It actually took me a while to understand what it meant with arithmetric sequence so i google it and tried to understand it.
Define- Once i understood I tried finding a way of solving it but i felt it was straight foward
Explore- I didnt know what structure to use to save the previous answers. But like usual i try to save them in the same structure as the problem is. It makes it easier
Aanticipate- I hoped for it to work and did the steps from duke for solving it by hand
Learn- I think i noticed that in this instance it is fasster and more intuitive using dynamic programming that normal.
