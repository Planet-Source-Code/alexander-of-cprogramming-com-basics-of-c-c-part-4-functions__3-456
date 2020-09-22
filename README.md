<div align="center">

## Basics of C/C\+\+ Part 4: Functions


</div>

### Description

Now that you have learned all about variables, loops, and if statements it is time to learn the next thing in programming: Functions. Obviously, you should have a good idea about what a function is, as you have used ones like cout before. However, this lesson will be more in detail about not only functions that are already made, but about making your own, or maybe I will continue this later...
 
### More Info
 


<span>             |<span>
---                |---
**Submitted On**   |
**By**             |[Alexander of CProgramming\.com](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByAuthor/alexander-of-cprogramming-com.md)
**Level**          |Beginner
**User Rating**    |4.3 (34 globes from 8 users)
**Compatibility**  |C, C\+\+ \(general\)
**Category**       |[Data Structures](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByCategory/data-structures__3-8.md)
**World**          |[C / C\+\+](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByWorld/c-c.md)
**Archive File**   |[](https://github.com/Planet-Source-Code/alexander-of-cprogramming-com-basics-of-c-c-part-4-functions__3-456/archive/master.zip)





### Source Code

<p> <font face="Verdana">    A good way to describe a
function is to show its prototype. That means, what it should return, and what
it should take as an argument. For example, the prototype of getch() is... int
getch(void); The int means that it returns an integer, the void means that it
does not take an argument. Now, you may know that getch returns a character!
However, that does not mean it must return a character. The fact that the return
type is an integer makes no difference, because the ASCII character set does not
care what type of number it is, as long as it is a number...don't worry if you
don't understand, it is not too important right now.</font></p>
<p><font face="Verdana">     What is important is that you
understand prototypes. Another prototype is... int kbhit(void); It returns an
integer, and it takes no value. Now that I hope you understand this then you
will be able to use the help files much more easily, and I can go into more
about functions.</font></p>
<p><font face="Verdana">     First, what functions are
useful. There are many useful functions, and often they are hard to find. For
Turbo C++ Lite some useful functions include, but are no limited to:</font></p>
<p><font face="Verdana">cout<< iostream.h output</font></p>
<p><font face="Verdana">cin>> iostream.h input</font></p>
<p><font face="Verdana">int getch(void) conio.h get characters</font></p>
<p><font face="Verdana">void clrscr(void) conio.h clear screen</font></p>
<p><font face="Verdana">     Okay, you might be thinking
that this is nothing! Four measly functions, and you are right! If there were
only a few functions then C/C++ would not be useful. However, a lot of programs
do not need all that many functions. Of course, I suggest that you know ever
function that you can, or at least the name. For this purpose, I will be posting
an entire listing of ever function that I can find out of either help or books I
have read. However, for now, these are probably the most useful functions. After
all, if you can clear the screen, get input and output, and get keypresses,
which are useful for stopping the program from immediately going back to the IDE
you can do quite a bit! Believe me, there are a few specialized, but very useful
funcitons, the thing is, you don't really need to use them all the time! If you
have a problem with a function that you need, and I have not put up my list yet,
then email me at lallain@concentric.net, and I will find you what you need!</font></p>
<p><font face="Verdana">     Anyway, after that long spiel
on not needing a lot of functions, I am going to show you how to make your own
functions! Wow, I can do that? Of course, otherwise C/C++ would not be useful!
So, prepare to learn how to make functions.</font></p>
<p><font face="Verdana">     First let me give you an
entire example program. Then we will look at it, and learn how to make our own
programs.</font></p>
<p><font face="Verdana">#include <iostream.h></font></p>
<p><font face="Verdana">#include <conio.h></font></p>
<p><font face="Verdana">int mult(int x, int y);</font></p>
<p><font face="Verdana">void main()</font></p>
<p><font face="Verdana">{</font></p>
<p><font face="Verdana">int x, y;</font></p>
<p><font face="Verdana">cout<<"Input a number, and what number to
multiply it by";</font></p>
<p><font face="Verdana">cin>>x>>y;</font></p>
<p><font face="Verdana">cout<<endl<<mult(x, y);</font></p>
<p><font face="Verdana">getch();</font></p>
<p><font face="Verdana">}</font></p>
<p><font face="Verdana">int mult(int x, int y)</font></p>
<p><font face="Verdana">{</font></p>
<p><font face="Verdana">return x*y;</font></p>
<p><font face="Verdana">}</font></p>
<p><font face="Verdana">     How is this useful...Well, in
this program the function is totally useless, and it can only multiply integers!
But this is just to show you how to make functions, after you understand the
basics I hope you will be able to do anything yourself.  What my example
does: #includes...basic includes What is int mult(int x, int y); ? That is a
prototype of the function, without it you would not be able to use mult! What is
void main()? You should know that. What is cout<<endl<<mult(x,y);
Well, basically it puts us down a line, and then it outputs what mult returns.
More on this later. What is</font></p>
<p><font face="Verdana">int mult(int x, int y)</font></p>
<p><font face="Verdana">{</font></p>
<p><font face="Verdana">return x*y;</font></p>
<p><font face="Verdana">}</font></p>
<p><font face="Verdana"> </font></p>
<p><font face="Verdana">     Well, it is a function! It says
that the return type is an integer. When the keywork return is used it says that
the function mult has a value of whatever x*y would be...as it says return x*y.
The two ints that it takes are x and y. So it multiplies them and returns that
value. Then outputs mult(x, y); It is perfectly legal. Perhaps it would help if
you think of it as saying that the function mult has a value of whatever
x*y is. This is not true really, it just returns that value, and you can do
whatever you want with it, but I hope it helps.</font></p>
<p><font face="Verdana">What can you do? You can make void functions that do
anything...</font></p>
<p><font face="Verdana">#include <iostream.h></font></p>
<p><font face="Verdana">void function(void);</font></p>
<p><font face="Verdana">void main()</font></p>
<p><font face="Verdana">{</font></p>
<p><font face="Verdana">function();</font></p>
<p><font face="Verdana">}</font></p>
<p><font face="Verdana">void function(void)</font></p>
<p><font face="Verdana">{</font></p>
<p><font face="Verdana">cout<<"This is a useless and totally wasteful
function";</font></p>
<p><font face="Verdana">}</font></p>
<p><font face="Verdana">What is does is declare that there is going to be a
function, by prototyping, and then at the bottom the function is defined, and it
only does one thing...outputs "This is a useless and totally wasteful
function" However, what if you wanted to do something that took 3 lines
four hundred times in different places? Say,</font></p>
<p><font face="Verdana">#include <iostream.h></font></p>
<p><font face="Verdana">void function(void);</font></p>
<p><font face="Verdana">void main()</font></p>
<p><font face="Verdana">{</font></p>
<p><font face="Verdana">LOTS OF CODE THAT NEEDS TO OUTPUT Line 1Line 2Line 3</font></p>
<p><font face="Verdana">}</font></p>
<p><font face="Verdana">void function(void)</font></p>
<p><font face="Verdana">{</font></p>
<p><font face="Verdana">cout<<"Line 1";</font></p>
<p><font face="Verdana">cout<<"Line 2";</font></p>
<p><font face="Verdana">cout<<"Line 3";</font></p>
<p><font face="Verdana">}</font></p>
<p><font face="Verdana">That, aside from the fact that it is a bad example, is
where you would use it. When you need to call something a lot of times, but
don't want to cut and paste. Functions are very useful, and I hope I explained
them well enough for you to understand.</font></p>

