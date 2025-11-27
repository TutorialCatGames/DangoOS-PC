# DangoOS-PC
Dango README v. 1.198 11/27/2025 M/D/Y
ALL VERSIONS ARE IN THE RELEASES TAB. https://github.com/TutorialCatGames/DangoOS-PC/releases/
1. Debugging
   1.1. debug()
   1.2. stdebug()
   1.3. print(any)
   1.4. start()
2. Statements
   2.1. if(var operator var, length)
3. Loops
   3.1. repeat(int, length)
   3.2. forever
4. Operators
   4.1. plus(any, any)
   4.2. minus(any, any)
   4.3. divide(any, any)
   4.5. random(any, any)
   4.6. multiply(any, any)
   4.7. mod(any, any)
   4.8. sqrt(any)
5. Inputs
   5.1. ask(string)
6. Variables
   6.1. let string = any
   6.2. output
   6.3. answer
   6.4. Starting Variables
   6.41. mx
   6.42. my
   6.43. md
7. Pen
   7.1. pendown()
   7.2. penup()
   7.3. clear()
   7.4. forward(int)
   7.5. turn(int)
   7.6. turnfor(int, int)
   7.7. moveto(int, int)
   7.8. color(int, int, int)
   7.9. point(int)
8. Screen
   8.1. window()
9. Separators
   9.1. dango()
10. Trigonometry
   10.1. sine(int)
   10.2. cosine(int)
   10.3. angt(int, int)
   10.4. tan(int)
   10.5. atan(int)
11. Stopping
   11.1. sleep(seconds)
   11.2. stforever()
12. String
   12.1. concat(string, string)
   12.2. letter(int, var)
   12.3. includes(string, var)
   12.4. startswith(string, var)
   12.5. index(string, var)
   12.6. len(var)
   12.7. shush(string)
   12.8. scream(string)
13. Algebra
   13.1. log(int)
   13.2. expo(int, int)
   13.3. e(int)
14. Rounding
   14.1. round(int)
   14.2. abs(int)
Challenges
   1. Calculator
   2. Exponents
Challenge Keys
   1. ...
   2. ...



IMPORTANT! To stop DANGO projects you need to hit the "end" key and release. After you release the key there will be a confirmation box. 
Click yes to stop the project and to make the confirmation box disappear. Click no to make the confirmation block disappear and still have the project running.




Command Station commands
1. clear # clears the list called "words"

2. close # asks "close" and closes the app that has the display name of the user's answer

3. restart # restarts the DangoOS

4. date # puts the date variable in local storage in to the words list. D/M/Y
5. dconfig # asks "dconfig" then configures the date variable in local storage to be the user's answer. The date can be anything.

6. currentdate # puts the current date in to the words list. D/M/Y

7. dir # puts all the files the user has in to the words list. 

8. copy # asks for the name (not display name) of the file the user want's to copy then asks for the display name for the new copied file. Then copies the file and makes the display name the answer variable.

9. bootinfo # puts any errors with the startup in the words list. If there aren't any it puts "No errors found." in the words list.

10. del # asks "del" and deletes the file with that display name.

11. create # asks "filename" and creates a dango file with the display name of the answer variable.

12. repcode # asks "displayname" then replaces the file with that display name's code with the latestcode list.

13. fastbooton # turns turbo mode on which makes everything faster. Turbo mode is off by default

14. fastbootoff # turns turbo mode off. Turbo mode is off by default

15. framecap # asks "framecap" and if the answer variable is a number it makes the max amount of frames the absolute value of the answer variable. And if the answer variable isn't a number it puts "answer" can't parse in to the words list.

16. dango # clears the screen makes everything you type after you typed "dango" go in to the latestcode list. enter "end" to go back to normal mode.



Reserved words:
output, answer, mx, my, md



Debugging:

1. debug() # shows these lists:
words,
variables,
operators,
latestcode,
repeat_idx,
var_values,
repeat_times

example:
let a = 5
debug()
print(a)


2. stdebug() # hides these lists:
words,
current,
first part,
variables,
operators,
latestcode,
repeat_idx,
var_values,
repeat_times

example:
stdebug()
repeat(288, 1)
turnfor(1, 1)


3. print(any) # print can print variable values. print can also be displayed as print("<str>") that can NOT display variables but can print integers, floats, and strings. the output will be displayed in the words list.

example:
print("1")


4. start() # start resets everything. It deletes everything from every list that are used in dango, hides them, sets the pen color to black/color(0, 0, 0) and sets pen transparency to 0%/makes the pen completely visible.

example:
start() # resets everything
concat(erm , what the sigma)
print(output) # prints erm what the sigma



Statements:

1. if(var operator var, length) # if conditions can't use math conditions inside of the if condition. They need to be this exact syntax and needs a space right after the comma. The length is how many lines below it are gonna be affected by the if statements. The first and second part are exclusively variables.
The operators supported below are the ones on the right.

(==) : (=)
(>)  : (>)
(<)  : (<)
(>=) : (#) # its like this "#" because of letter by letter viewing.
(<=) : (@) # its like this "@" because of letter by letter viewing.

example:
let a = 2
let b = 5
if(a > b, 1) # this will not print the one below
print("haha")

WARNING! The if condition as of DangoOS v. 0.9.2 can only be used once per project. If you use two of them both conditions will be true regardless if its false or not. Please refrain from using 2 if conditions right now.



Loops:


1. repeat(int, length) # runs the block of code inside it exactly int times. each time the loop runs is called an iteration. after finishing one iteration, it moves to the next until it has repeated the block the specified int of times. if int = 0, the code inside will not run at all. length = number of lines affected below the repeat

example:
repeat(1, 1)
print("haha")


2. forever # anything after this forever loop gets repeated forever.

example:
forever
print("haha") # this will lag



Operators:


1. plus(any, any) # this operator adds the first and second input. This can read variable values but can't join two strings. The output is outputted to a variable named "output".

example:
plus(1, 1)
let a = output # a will be 2


2. minus(any, any) # this operator subtracts the first and second input. This can read variable values but can't join two strings. The output is outputted to a variable named "output".

example:
minus(123, 55)
let b = output # b will be 68


3. divide(any, any) # this operator divides the first and second input. This can read variable values but can't join two strings. The output is outputted to a variable named "output".

example:
divide(1, 2)
let c = output # c will be 0.5


4. random(int, int) # this operator picks a random number between the first and second int or float. This can read variable values but can't join two strings. The output is outputted to a variable named "output".

example:
random(1, 56)
let d = output # d will be a number between 1 and 56


5. multiply(any, any) # this operator multiplies the first and the second input. This can read variable values but can't join two strings. The output is outputted to a variable named "output".

example:
multiply(547, 2)
let e = output # e will be 1094


6. mod(any, any) # this operator gets the remainder from subtracting the first and second input. This can read variable values but can't join two strings. The output is outputted to a variable named "output".

example:
mod(2, 123)
let f = output # f will be 2


7. sqrt(any) # this operator gets the square root of the first input. This can read variable values but can't join two strings. The output is outputted to a variable named "output".

example:
sqrt(144)
let g = output # g will be 12



Inputs:

1. ask(string) # this input block will only have the string as a variable. This can also be put as ask("string") where this time it can only be a string and nothing else. the output will be outputted to a variable named "answer".

example:
ask("hello") # in this example the user inputted "hi"
let a = answer
if(a = hi, 1)
print("yay")



Variables:


1. let string = int # this is the syntax to make or edit a variable in the Dango programming language. You can't use it like this:
"let string = 1 + 1." To add or use any operators you need to use it like this:
"plus(1, 1)
 let string = output."

example:
let haha = 1
print(haha) # this will print "1"


2. output # output is the variable that operators outputs to.

example:
plus(1, 123) # the answer will be put inside the variable "output"
let asda = output


3. answer # answer is the variable that the "ask(string)" block outputs to.

example:
ask("hello") # the answer got outputted to the answer variable
let a = answer
if(a = nuh uh)
print(":(")


Starting Variables:

1. mx # the variable that always is equal to the x axis of the mouse.

example:
random(-280, 280)
moveto(mx, output) # uses mx


2. my # the variable that always is equal to the y axis of the mouse.

example:
if(my = 280, 1)
print("280")


3. md # the variable that is 1 if the mouse is down and 0 if not.

example:
print(md)
if(md = 1, 1)
print("mouse is down")
if(md = 0, 1)
print("mouse is not down")



Pen:


1. pendown() # the block that makes it so that you have a pen trail behind the sprite

example:
pendown()
moveto(-180, 189)


2. penup() # the block that disables/turns off the pen trail behind your sprite

example:
penup()
moveto(0, 0)
point(90)
pendown()
forward(65)


3. clear() # the block that deletes all pen trails.

example:
penup()
clear()
color(0, 0, 0)


4. forward(<int>) # makes your sprite go <int> steps in the direction its facing. If the pen is currently down it makes a line from your old position to your new position.

example:
pendown()
repeat(10, 1)
forward(10)
repeat(10, 1)
forward(-15)


5. turn(<int>) # makes your sprite turn clockwise by <int> steps.

example:
penup()
point(90)
pendown()
turn(45)
repeat(180, 1)
forward(1.51)


6. turnfor(<int>, <int>) # makes your sprite go <int> steps in the direction its facing from the first input. If the pen is currently down it makes a line from your old position to your new position. And turns clockwise <int> degrees from the second input.

example:
clear()
repeat(288, 1)
turnfor(3, 3)


7. moveto(<int>, <int>) # makes your sprite's x position to be the first input and the y position to be the second input. If the pen is currently down it makes a line from your old position to your new position.

example:
moveto(0, 0)
repeat(3, 1)
turnfor(50, 120)


8. color(<int>, <int>, <int>) # makes the pen color <int>, makes the pen saturation <int>, and makes the pen brightness <int>. 

example:
color(255, 255, 255)
pendown()
repeat(3, 1)
forward(12)


9. point(<int>) # makes your sprite angle <int>.
90  : right
-90 : left
180 : down
0   : up

example:
point(90)
turn(45)
repeat(105, 1)
forward(1)


Screen:


1. window() # adds a window with a white background and a black outline to your screen. If you try to put the sprite outside of bounds it clamps the x and y position. This window can't be moved as of right now (DangoOS v. 0.9.2.)
Horizontal bounds: -144 to 142. 
Vertical bounds: -125 to 123.


example:
start()
window()
moveto(0, 0)
forward(100) # this will still be in bounds and not touch the corner since the bounds are bigger than 100 px.



Separators


1. dango() # a line of code that will execute the code before it. Can only take some lines of code.

example:
moveto(105, 105)
forever
turnfor(1, 0.5)
dango()



Trigonometry


1. angt(int, int) # this trigonometric operator gets the angle that will point at the first and second input using this formula:
(atan(((first input) - (x position)) / ((second input) - (y position))) + ((180) * <(second input) < (y position)>)).
But in dango it would look like this (without using angt()):

let x = 0
let y = 0
let otherx = 90
let othery = 0
minus(otherx, x)
let fp = output
minus(othery, y)
let sp = output
divide(fp, sp)
atan(output)
let dir = output
if(othery < y)
plus(dir, 180)
let dir = output

This can read variable values but can't join two strings. The output is outputted to a variable named "output".

example:
angt(280, 0) # in this example x position = 0, y position = 0
let a = output # a will be 90


2. sine(int) # this trigonometric operator returns the sine of the int input in degrees. The output is outputted to a variable named "output".

example:
sine(0)
let b = output # b will be a float: 0.000...


3. cosine(int) # this trigonometric operator returns the cosine of the int input in degrees. The output is outputted to a variable named "output".

example:
cosine(1)
let c = output # c will be a float: 0.54030230586


4. tan(int) # this trigonometric operator returns the tan of the int input in degrees. The output is outputted to a variable named "output".

example:
let taninput = 124
tan(taninput)
let d = output # d will be a negative number: -1.4825609685


5. atan(int) # this trigonometric operator returns the atan of the int input in degrees. The output is outputted to a variable named "output".

example:
let trigonometric = -1
atan(trigonometric)
let e = output # e will be a negative number: -45



Stopping


1. sleep(seconds) # a line of code that will stop the project for <input> seconds. This is inputted directly in the run Dango Interpreter.
 
WARNING! This command is still not perfected yet. The interpreter will lag if you run this command. Please wait for it to be fixed to work.

example:
forever
print("1") # this can be print(1) but some errors might happen.
sleep(0.1) # lags


2. stforever() # this line of code stops the project forever and makes everything disappear.


example:
plus(60, 4)
print(output) # outputs 64 to the words list.
sleep(10) # lags
stforever() # stops the project forever



String


1. concat(string, string) # this string operator joins the first and second string inputs. This can't read variable values and can't join anything except strings. The output is outputted to a variable named "output".

example:
concat(a, a)
let a = output # a will be aa


2. letter(int, var) # this string operator finds the letter int input of the var input. The output is outputted to a variable named "output".

example:
concat(hello, world!)
let x = output
letter(4, x)
let b = output # b will be l


3. includes(string, var) # this string operator finds out if the string input is in the var input. The output is outputted to a variable named "output".

example:
concat(erm what, the sigma)
let x = output
includes(haha, x)
let c = output # c will be 0


4. startswith(string, var) # this string operator finds out if the var input starts with the string input. The output is outputted to a variable named "output".

example:
concat(good, morning:D)
let x = output
startswith(good, x)
let d = output # d will be 1


5. index(string, var) # this string operator finds out the index of the string input in the var input. The output is outputted to a variable named "output".

example:
concat(do you hear, the whistle?)
let y = output
index(d, y)
let e = output # e will be 1


6. len(var) # this string operator finds out the length of the var input. The output is outputted to a variable named "output".

example:
concat(bread , tastes good:D)
let z = output
len(z)
let f = output # f will be 19


7. shush(string) # this string operator makes the string input lowercase. The output is outputted to a variable named "output".

example:
concat(STOP USING , CONCAT PLEASE)
let a = output
shush(a)
let g = output # g will be stop using concat please


8. scream(string) # this string operator makes the string input uppercase. The output is outputted to a variable named "output".

example:
concat(gr , r)
let idkman = output
shush(idkman)
let h = output # h will be GRR



Algebra


1. log(int) # this algebraic operator gets the log10() value of the int input. The output is outputted to a variable named "output".

example:
log(10)
let logout = output # logout will be 1.


2. expo(int, int) # this algebraic operator makes the output to be the <int> input to the power of the second int input. The output is outputted to a variable named "output".


3. e(int) # this algebraic operator gets the value of e/Euler's number  (2.718281828459045) to the power of the int input. The output is outputted to a variable named "output".



Rounding


1. round(int) # this rounding operator rounds the int input to the closest whole number. The output is outputted to a variable named "output".

example:
round(3.14159265)
let rpi = output # rpi will be 3.

2. abs(int) # this rounding operator gets the absolute value of the int input. The output is outputted to a variable named "output".

example:
let negative = -1315
abs(negative)
let absolute = output # absolute will be 1315






Challenges


1. Calculator 
With the Inputs, Debugging and Operators categories, try and make a mini calculator with them. You are not permitted to use any other category.

Bonus:
Make the calculator able to calculate trigonometric calculations. No trigonometric operations.


2. Exponents
With only the Loops and operations category, try and make a program that calculates the expo() command.

Bonus:
Add factorials. And make all of it under fifteen lines.




Hints: 


1. Calculator
Use Operators, they will help. minus(), plus() and more will lead you


2. Exponents
Try to use multiplication it might help.
