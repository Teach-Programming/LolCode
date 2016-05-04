#1. INTRODUCTION


We're going to be using a website called www.repl.it to have fun with lolcode.

* Open repl.it (ctrl-left click or right click and open in a new tab) [repl.it/languages/LOLCODE](http://repl.it/languages/LOLCODE)

Don't forget the buttons in the top bar regularly:

* Run - when you want to test your code

* Save - when you think it works and you wanna share


![Imgur](http://i.imgur.com/l3EsgJk.png)


![catz](http://www.lolcats.com/images/u/11/46/lolcatsdotcomqc2oos4nrd7aymcl.jpg)


#2. OUTPUT

```VISIBLE``` prints to the standard output. 

So our ubiquitous 'Hello World' program becomes:

```
HAI 1.2
    VISIBLE "HAI, WORLD!!!
KTHXBYE
```

*Add hip comments to your code using BTW for single line comments and OBTW / TLDR for multiline comments, like in my hello world program below.*


![Imgur](http://i.imgur.com/Gc6oLcE.png)

![catz](http://www.lolcats.com/images/u/07/35/lolcatsdotcom8514whl5iwcfrm1k.jpg)

#3. INPUT

Variables are declared using ```I HAS A```, and the variables can be initialized on the same line using using ```ITZ```.

Or we can ask the user for values using ```GIMMEH```. In some systems it brings up a modal dialog box, other systems wait for command line entry.

```
HAI 1.2
    I HAS A KITTEH
    GIMMEH KITTEH
    VISIBLE "HAI, ", KITTEH
KTHXBYE
```

*repl.it waits on the command line, as you can see when I run my program below:*


![Imgur](http://i.imgur.com/lAlxL1r.png)


![catz](http://www.lolcats.com/images/u/08/50/lolcatsdotcomrq4lywopmz2tyzsb.jpg)

#4. CONDITIONALS

The conditional ```if (Var1 == Var2){}``` is represented as ``` BOTH SAEM Var1 AN Var2``` and ``` O RLY?```, on a new line.

The true condition has ```YA RLY``` and, of course, you can do nested conditions with ```GIMME```. Like in the example below:

```
HAI 1.2

I HAS A ANIMAL
GIMMEH ANIMAL

BOTH SAEM ANIMAL AN "CAT"
O RLY?
    YA RLY, VISIBLE "J00 HAV A CAT"
    MEBBE BOTH SAEM ANIMAL AN "MAUS"
        VISIBLE "NOM NOM NOM. I EATED IT."
OIC

KTHXBYE
```

*I hope you liek the cool cat code, the results from my program look like this:*


![Imgur](http://i.imgur.com/LoJEg1O.png)


![catz](http://www.lolcats.com/images/u/08/51/lolcatsdotcomo1gehe7hiqmn05ig.jpg)

#5. SWITCH STATEMENTS

Multiple conditions can usually be written more neatly  as a Switch/Case statement, this is represented as ``` Var, WTF? and OMG Val``` for the switch / case.

So, the nested conditions of the cat & mouse game from the previous slide can be rewritten like the example below:


```
HAI 1.2
I HAS A KITTEH
GIMMEH KITTEN

KITTEH, WTF?
    OMG "CAT"
       VISIBLE "J00 HAV A CAT"
       GTFO
    OMG "MAUS"
       VISIBLE "NOM NOM NOM. I EATED IT."
       GTFO
    OMGWTF
OIC

KTHXBYE
```


*The results from my code look like this:*

![Imgur](http://i.imgur.com/nBedbq1.png)

![catz](http://www.lolcats.com/images/u/08/30/lolcatsdotcomdoozp810tzfcq0up.jpg)

#6. LOOPS

Loops are a succinct way of representing repetition, this is represented as ''' IM IN YR LOOP / IM OUTTA YR LOOP'''.

So, the classic game of 'I ate a ...' can be rewritten like this:


```
HAI 1.2

I HAS A KITTEH ITZ "Katz"
I HAS A IDIOT ITZ 0

IM IN YR LOOP UPPIN YR IDIOT TIL BOTH SAEM AN 10
   BOTH SAEM IDIOT AN 8, O RLY?
      YA RLY
         VISIBLE "COOL, I ATE A ", KITTEH
      NO WAI
         VISIBLE "COOL! I " IDIOT " A " KITTEH
   OIC
IM OUTTA YR LOOP

KTHXBYE
```

*The results from my code look like this:*


![Imgur](http://i.imgur.com/fHFRust.png)

![catz](http://www.lolcats.com/images/u/11/45/lolcatsdotcom3gp6wm7dw3jihq9t.jpg)

#7. FUNCTIONS

Functions are a useful way of putting statements together, so that they are easier to understand and reduce the amount of typing you have to do.

Functions are declared using ``` HOW DUZ I FunctionName YR Var / IF U SAY SO```

So, our cat & mouse game can be refactored like this:

```
HAI 1.2

HOW DUZ I TASTEH YR BEAST

BEAST, WTF?
    OMG "CAT"
       VISIBLE "J00 HAV A CAT"
       GTFO
    OMG "MAUS"
       VISIBLE "NOM NOM NOM. I EATED IT."
       GTFO
    OMGWTF
OIC

IF U SAY SO

I HAS A ANIMAL
GIMME ANIMAL

TASTEH ANIMAL

KTHXBYE
```

*The results of my code look like this:*


![Imgur](http://i.imgur.com/HIbI1Rr.png)

![catz](http://www.lolcats.com/images/u/11/49/lolcatsdotcomii0sbc7g7dpgu21m.jpg)

#8. A LOL APP

Ok, even though Lolcode is Turing complete, some people don't believe that it is a proper language, so here after all the games let's do some proper work!

Everybody knows the Fibonacci Sequence, named for Leonado Pisano, who brought the Arabic numerals into European mathematics and the superior technology of Arabic arithmetic that we all learn today.

Fun fact: Leonado Pisano, also known as Fibonacci (son of Bonacci), did absolutely nothing with the sequence that bears his name. But never mind, Fibonacci deserves to be remembered for his great contribution to numberacy.

The sequence is 1 1 2 3 5 8 13 21 - each number is given as the some of the previous 2 numbers. 1 + 1 = 2, 1 + 2 = 3 etc

* This neatly gives the generating function of the sequence,

It ain't Poetry but it seems to work - it gives:

* Fibonacci rule F_n = F_{n-1} + F_{n-2}.

Which we can program easily with a function that calls itself twice!

```lolcode
HAI 1.2

HOW DUZ I FIBONACCEH YR NUMBEH
  
  I HAS A NUMBE
  I HAS A NUMB
  I HAS A NUMNUM
  NUMBE R DIFF OF NUMBEH AN 1
  NUMB R DIFF OF NUMBE AN 1
  
  NUMBEH, WTF?
    OMG 0
       FOUND YR 0
       GTFO
    OMG 1
       FOUND YR 1
       GTFO
    OMGWTF
       NUMNUM R SUM OF FIBONACCEH NUMBE AN FIBONACCEH NUMB
       FOUND YR NUMNUM
       GTFO
  OIC
IF U SAY SO

I HAS A LOLCAT ITZ 16
I HAS A VAR ITZ 1

IM IN YR LOOP UPPIN YR VAR TIL BOTH SAEM VAR AN SUM OF LOLCAT AN 1
   	VISIBLE FIBONACCEH VAR
IM OUTTA YR LOOP

KTHXBYE
```

Unfortuantely, the Lolcode syntax isn't very polished, so I have to declare two intermediate variables to store the values of the previous calls to the Fibonacceh function. Meh.

*My code and the results of running it look like this:*

![Imgur](http://i.imgur.com/f9BCX05.png)

![catz](http://www.lolcats.com/images/u/11/49/lolcatsdotcomii0sbc7g7dpgu21m.jpg)

#9. Challenges

Some programming fun, coding challenges:

* A. Code a generator for '10 green bottles'


```
10 Green Bottles sitting on the wall,

if one green bottle should accidentally fall,

there'll be 9 green bottles sitting on the wall
...
```

It's quite good fun to go to -10 green bottles, and then count up again.


* B. Code a generator for a binary search

Python can do the [**binary search**](http://openbookproject.net/thinkcs/python/english3e/list_algorithms.html) like this:

```python
def search_binary(xs, target):
    """ Find and return the index of key in sequence xs """
    lb = 0
    ub = len(xs)
    while True:
        if lb == ub:   # If region of interest (ROI) becomes empty
           return -1

        # Next probe should be in the middle of the ROI
        mid_index = (lb + ub) // 2

        # Fetch the item at that position
        item_at_mid = xs[mid_index]

        # print("ROI[{0}:{1}](size={2}), probed='{3}', target='{4}'"
        #       .format(lb, ub, ub-lb, item_at_mid, target))

        # How does the probed item compare to the target?
        if item_at_mid == target:
            return mid_index      # Found it!
        if item_at_mid < target:
            lb = mid_index + 1    # Use upper half of ROI next time
        else:
            ub = mid_index        # Use lower half of ROI next time

```

Can you write it in Lolcode?


![Imgur](http://i.imgur.com/8bAz4i6.jpg)



