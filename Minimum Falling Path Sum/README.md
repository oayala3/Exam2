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
if(locationX==A.lenght-1) call the funtion on findAll(x,y+1,A) and findAll(x-1,y+1,A)  
else findAll(x,y+1,A) and findAll(x-1,y+1,A) and findAll(x,y-1,A)  
  
else
min=arr[x][y]
arr[x][y]=min
return min  
  
The general idea id to traverse trhough the whole 2d array. Before you call the funtion again check if the answerArray has something in the location. Use that if there is, if not call the funtion.  
  Step 2
  I plan to save the prevous solutions on a globar int[][]. It will be populated before the returns. 
  Since it has the same structure as the original, checking is easy. Before you call the funtion you can check if the answer array has something saved there.
    
  Step 3  
  Since i am more of a hands on learner. I DUKE helps alot. The step one is solving the probelem by hanh and step 2 is writing down what you did. So i did that on paper. Then noticed that it was easy using cordiantes. So i generalized the problem to the three possible things, Left edge right edge or middle. 
