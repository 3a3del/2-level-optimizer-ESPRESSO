# 2-level-optimizer-ESPRESSO
# ESPRESSO OVERVIEW
ESPRESSO is a tool originally developed at the University of California at Berkeley by Rick Rudell, Bob Brayton, and Alberto Sangiovanni-Vincentelli.
You will find two helpful tutorials about ESPRESSO: a written document that explains the tool and its capabilities, and also a short video tutorial about to use ESPRESSO in (https://www.youtube.com/watch?v=dXuCLx4kwfY). Please go look at those before you proceed further in this.  
Reduce-Expand-Irredundant cycle.
• Reduce 
  - Rank cubes in a clever order, do PCN bit hacking to reduce them individually 
• Expand 
  - Rank cubes in the opposite of this clever order, expand each individually as a pair of covering problems 
• Irredundant                     
  - A clever URP algorithm (like tautology) + a clever covering problem 
And a bunch of other interesting steps we did not mention...
What a real 2-level optimizer can do !
# Description
Assuming you have read/viewed these tutorial materials.Suppose we have a function 𝐹 ( 𝑥 1 , 𝑥 2 , 𝑥 3 , 𝑥 4 , 𝑥 5 , 𝑥 6 ) F(x 1 ​ ,x 2 ​ ,x 3 ​ ,x 4 ​ ,x 5 ​ ,x 6 ​ ). We set 𝐹 = 1 F=1 if there are exactly 2 1’s, or 3 1’s, or 4 1’s in the input variables, else we set 𝐹 = 0 F=0. So, for example, 𝐹 ( 1 , 1 , 1 , 0 , 1 , 0 ) = 1 F(1,1,1,0,1,0)=1, because we see 4 1’s. And we set set 𝐹 ( 0 , 1 , 1 , 0 , 0 , 0 ) = 1 F(0,1,1,0,0,0)=1, because we see 2 1’s. But 𝐹 ( 0 , 0 , 0 , 0 , 0 , 1 ) = 0 F(0,0,0,0,0,1)=0, because see only one 1. Similarly, 𝐹 ( 1 , 1 , 0 , 1 , 1 , 1 ) = 0 F(1,1,0,1,1,1)=0 because we see 5 1’s, (This is small enough you can type it, it’s just a little bit boring).        

# Results
By Looking at the output result
- All AND gates in this 2-level ESPRESSO design have 4 inputs!!, From 6 inputs at each AND gate in the 2 level SOP to 4 therefor lower input wires, literals so lower hardware complexity, lower used Area, lower cost, higher design to market                    
You can try this with anathor implementaion logic and tell how a real 2-level optimizer can do !

                                                                                                    
  
  
  
  
  
  
  
  
  
  
