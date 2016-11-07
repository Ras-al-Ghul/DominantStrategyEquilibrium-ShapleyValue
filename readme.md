#Dominant Strategy Equilibria and Shapley Value

###Dominant Strategy Equilibria

To run `python DSE.py <input nfg filename>`  

This is python code to find a strongly as well as weakly dominant strategy equilibrium of `any n person matrix form game`. (For input, generate games of `.nfg` file format of `gambit`) <http://www.gambit-project.org/gambit14/formats.html>  

**Input file format:**  
Please note that the input nfg file shouldn't have a trailing space.  
Also, we've used `zero based indexing` The numbering starts from zero.  
The first line should contain the game name, and the second line should have the player names, followed by the number of strategies of each player.  
Third line should be blank, and the 4th line should contain all the payoffs as stated for nfg files on the Gambit website.  
Please ensure that there are no trailing spaces for the program to function properly.  
An `example.nfg` has also been provided which has a `Strongly Dominant Strategy Equilibrium` at strategy 1 (second strategy) for Player1, strategy 2 (third strategy) for Player 2 and strategy 3 (fourth strategy) for Player 3 (Note the zero based indexing)  

###Shapley Value

To run `python shapley.py <filename>`  

This is python code to compute a Shapley Value of a `characteristic form game`.  

**Input file format:**  
N = n  
v(1),...,v(1,2,….,n)  

( Number of players in the first row and valuations for all the coalitions in the second row except the empty set. Valuations are ordered in this manner: v(1),..,v(n),v(12),..,v(1n),v(23)..,v(2n),..,v(n-1n),v(123),v(124),.,v(12n),v(234)..,..,v(12..n) )  
An `example` file has been provided which is for the `Divide the Dollar version 2` game from Prof. Y. Narahari's Game Theory lecture notes <http://lcm.csa.iisc.ernet.in/gametheory/ln/web-cp3-TUgames.pdf>
