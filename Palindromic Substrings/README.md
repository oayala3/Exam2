**Describe**
Given a string, your task is to count how many palindromic substrings in this string.  
The substrings with different start indexes or end indexes are counted as different substrings even they consist of same characters.  
Something to Note is that a palidrome can be "a" or "aa" or "aaa"  
Also part of the probem is that even if the same charecters are used, as long as they are in different locations it counts as one more  
**Solution**
The solution is checking all of the locations for palidromes. To do this you need a funtion boolean Palidrome() that takes 3 parameters, the string the left location and the right location.  
The funtion will ehck if left and right chars are the same. If they are move the left side +1 and the right side -1  while L<R. 
You will call the funtion for every location by doing a for(int L=0;L<str.legnth;L++) isnide of this you will call the fumtion on for(int R=0;R<str.legnth;R++). This way  
you will check for all of the possible substrings.  
Dynamically you can do this by finding the smallest possible cases. And adding on to those. You will use the palidrome of size 1 and 2 as base.  
Then you will check grow those bigger by checking one more to the Left and Right
  
Since you will store two things, you can use a 2d array with the dimentins of the string  
helleh

H _ _ _ _ _  
_ E _ _ _ _  
_ _ L _ _ _  
_ _ _ L _ _   
_ _ _ _ E _  
_ _ _ _ _ H   
^Found 6  
  
H _ _ _ _ _  
_ E _ _ _ _  
_ _ L L _ _  
_ _ L L _ _-This line will not be counted since its a double  
_ _ _ _ E _  
_ _ _ _ _ H  
^ found 6+1  
  
H _ _ _ _ _  
_ E _ _ _ _  
_ E L L E _  
_ E L L E _-This line will not be counted since its a double    
_ _ _ _ E _  
_ _ _ _ _ H  
^found 7+1  
  
H _ _ _ _ _  
_ E _ _ _ _  
H E L L E H  
H E L L E H-This line will not be counted since its a double    
_ _ _ _ E _  
_ _ _ _ _ H  
^found 8+1

  Step 3
Solving the problem by hand gave me an Idea. I hadnt noticed that a palidrome is made of a plaidrome in the inside.  
After noticing that the solution became really aparent. Use the two base cases and grow from there.
I think that DUKE has become part of my problem solving because that specific step helps you troubleshoot the problem faster. It opens your mind.  
