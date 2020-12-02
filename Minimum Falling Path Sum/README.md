#Step 1  
Define:  
A falling path starts at any element in the first row, and chooses one element from each row.  The next row's choice must be in a column that is different from the previous row's column by at most one.Example  
|      1  
|     /|\  
|    1 2 3  
Some things that I noted was that going down choosing the smallest onw you see cause you can enclose yourself with the highest numbers. Example  
1 2 3 4  
1 1 2 2  
9 9 9 1  
The smallest possible way to going to the bottom is by picking 3 then 2 then 1
Solution:  
The solution is to add all the values that you can get by doing

findAll(int x,int y, int[][] A)
create an array of the same dimentions
then 
for (A.leght)
locationX=i  
  
if(y+1<A[0].leght)  
if(locationX==0) call the funtion on findAll(x,y+1,A) and findAll(x+1,y+1,A)  
if(locationX==A.lenght) call the funtion on findAll(x,y+1,A) and findAll(x-1,y+1,A)  
else findAll(x,y+1,A) and findAll(x-1,y+1,A) and findAll(x,y-1,A)  
 
