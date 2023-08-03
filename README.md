# Minesweeper-using-first-order-Logic-Agent
I implement a logic agent that use pure "resolution" rule and "propositional logic" to solve the minesweeper game . 

The agent treat each cell as a symbol that can be either false ("safe") or true ("mined"). 

The game proceeds as the player continues to mark the cells as safe or mined . 

The initial game configuration is : Easy (9x9 board with 10 mines), Medium (16x16 board with 25 mines), and Hard (30x16 board with 99 mines). And we'll provide an initial list of "safe" cells for the agent to make some exploration . I use round(sqrt(#cells)) as the number of initial safe cells . 

The hardest part for this game is that we need to maintain our knowledge base(KB) containing CNF clauses , so that we can use "resolution" rule to complete the task . 

The rules to generate CNF clauses whenever a hint is provided to the agent is as followed : 
![image](https://github.com/za970120604/Minesweeper-using-first-order-Logic-Agent/assets/72210437/518a35c3-471a-4ab7-a636-1444663adae5)

Alongside the code is my analysis on the agent's behavior , named report.pdf .

The code is well commented and I recommend everyone to modify the code and see what's happening .


