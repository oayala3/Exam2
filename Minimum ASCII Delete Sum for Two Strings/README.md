Given two strings s1, s2, find the lowest ASCII sum of deleted characters to make two strings equal.  
Ascii charecters, like letters and other charecters have a value. This is the value you will be adding.  
**Solution**  
I feel like this is very similar to the house robber problem.  
So the solution is as follows.  
You will check if both of the string.charAt(i)==string2.charAt(i). If they are you need no change and you can advance  
if they are different then you need to call the funtion removing one and call the funtion removing the char in the other  
Then you pick the smallest adn repeat.
If you decide to do this in a dynamical way, You can save the answer of the smallest using **2 array**, like we did on the house problem  
You remove one in one and remove the other in the other. You calculte the results by comparing the smallerst every time. This will stop you from   
solving the same problem mulptiple times

**Step 3**  
This is an example of the last step of IDEAL because the learning part helps you. When i saw the problem  
I saw a pattern, Even if i havent tested the solution i feel like it is correct because of the lecture  
and the previous example 
