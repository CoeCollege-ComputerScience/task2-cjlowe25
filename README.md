Q1. The game allows the user to look around through specific commands in a console, every time it is
the user's 'turn', it tells the user every direction that they could go.
Q2. The three commands the game allows for is "Help" which reiterates your situation and gives you a
list of commands you can use. "Quit" which ends the program. And "Go" which if you put a valid direction
in front of it, you will be able to move to a different room.
Q3. There are current 4 rooms; The Campus Pub, A Lecture Theatre, 
Outside the Main Entrance of the University, A Computing Lab, and A Computing Admin Office
Q4. The Game class seems to be the main controller, it creates a parser object which is what is used to 
inputs from the user. Those parser outputs are sent to a command class which holds those answer values as something
to be called upon. Then the game class calls upon that command class to process the answers and figure out what the
program needs to do in response to the user inputs, if its a help or quit command, the game class handles it and
stops or provides help messages accordingly. If its a go command, then it uses the room classes that would've been
created earlier to change which 'room' the user currently is in according to the game class.
Q5. It seems a little over complicated for no reason, like the command and commandWords classes could easily just
have their functions be apart of some other class, like the game class.
Q6. 
ZuulWorld exists only to hold the main class and start the game
Room class handles everything related to what's in a room and the exits to a room
Parser class handles getting inputs from the user and converting them into specific variables for other classes to use
Command class takes the inputs from the parser class and stores them for future use
CommandWords class handles everything regarding the words the user would use, verifying they're valid, establishing them, etc.
Game class handles the effects of the commands from the user, it also handles the giving of information to the user
