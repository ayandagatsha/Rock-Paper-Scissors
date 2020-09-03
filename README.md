Rock Paper Scissors

1. Open the index file on the browser.
2. Open the dev tools and go to console.
3. Type 'game()' in the console.
4. Type rock, paper or scissors in the pop-up box that asks you to choose
   by typing. 

5. The game will calculate your choice and the computers choice then announce
   whose choice one before printing the point score. 

6. Step 4 to 5 will occur four more times and at the end, the scores will
   be evaluated and an announcement of a winner(highest score) or a 
   draw(equal score).

7. Rock beats scissors, scissors beats paper and paper beats rock. 
8. Your choice needs to beat the computers choice to score points and win. 

9. The computers choice is based purely on random selection using the 
   code below: 

      let options= ['rock', 'paper', 'scissors']

      function computerPlay(){
          
          let randChoice= options[Math.floor(Math.random()*options.length)];
          return randChoice;
          
      }

                    The code above is explained below

The computer, reading from left to right and top to bottom is told 
to group the words: rock, paper and scissors under the word 'options'.

Then, following the mathematics rules of calculating what is inside brackets
first, it reads 'Math.random()*options.length, which tells it to pick any 
random number with a decimal from the number of how many group of words 
there are in the word options. 

There are three. 
 
The manner in which the words are organized is that, the first word is 
given positon zero, the second word, one and so on.

The way Math.random works is by picking any random number with a decimal
except the last one. so it it was Math.random*1, the computer would 
pick a number between zero and one, but never pick one. 

So, given that there are three groups of words, but their positoning 
starts from zero, the computer pick a decimal number from zero to 
two point something and never three. 

The Math.floor that encapsulates the Math.random instruction, picks the 
highest nummber without a decimal in a whatever group of numbers. So 0.45
will be just 0. 

The computer will see those instructions for number picking encapsuled in the
word options and use the number to pick whether rock, paper, or scissors, 
given however they are ordered in their numbered positons from zero to two. 

Then that choice is placed in the word 'randChoice'.
and the computer is told by the return function to stop looking for any other
instructions but keep whatever random choice from rock, paper or scissors was
made and kept in randChoice. 

This whole process is kept in the word, 'computerPlay()'.

So when anyone types 'computerPlay()' in the console of a broswers devtools
with those instructions, the computer prints out, rock or paper or scissors.



The player gets to make their choice through the code below inserted in 
a specific place:

playerSelection = prompt('Choose by typing: rock, paper or scissors!') 

     NB: review index.html to see complete code.
