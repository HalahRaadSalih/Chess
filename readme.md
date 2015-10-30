### Chess Game using Java Script

##### Team members:

 - Halah 
 - Edward
 - Jonathan 


### Classes, their properties and thei methods

Here you will find the classes within the chess game and the properties of each one of them and their methods. All of them are subject to change as we go on with code, as you just saw in the exmple with the sandwich shop and how what her original map changed as she started coding.


Starting with a player!

### Player
- Name - > String to hold the player name
- Score -> a value of the current score
- Peices -> an array represents the number of peices a player has at the moment.


### Moves
1)Pieces
	a)  Rook -> moves in any number of squares in a vertical or horizontal direction. Maybe used to Castle with the King.
	b)  Knight -> moves in two ways: two squares horizontal and an offset of one square vertical, or two squares vertical and an offset of one square horizontal. Has the ability to "jump."
	c)	Bishop -> moves in any number of squares in a diagonal direction. 
	d)	Queen -> moves similarly to the Rook and Bishop.
	e)	King -> moves similarly to the Queen, but only occupies a square away from it's previous position.
	f)	Pawns -> moves in a linear fashion towards the opponent's side of the board. If it reaches the opponent's side of the board, it can use a special move called "Promotion". Once obstructed in it's path, pawn's can only move once again if the obstruction has been eliminated or if the Pawn itself is able to capture a piece in a one-square-diagonal path. It is the only piece that captures differently from the way they move. Also, pawns are not allowed to move backwards.
2)Special Moves
	a)  Promotion -> As the pawn reaches the side of the opponent, the pawn can be promoted to any other piece except for a king.
	b)	En Passant -> Is a special capture move that can only be used by a pawn, immediately after an opponent's pawn has moved two spaces. Once opponent's pawn is captured, the placement of the pawn differs as it "passes" the opponent's pawn by one square backwards in favor of the En Passant user.
	c)	Castling consist of a King moving two spaces towards either Rook, and moving the Rook on the other side of the King. A set of conditions need to be met:
		-The King and Rook involved must not have moved in the game.
		-There must be no obstructions/pieces within the path of the King and Rook.
		-The King must not be in Check.
	d)	Check -> A king is under attack by one or more enemy piece. A piece may also be unable to move if the piece will deliver a Check to the mover's King. If the King is in Check, the King must either move to safety, block the piece that threatens the king, or capture the piece that threatens the King. Once Checked, all other moves are considered invalid if it doesn't change the King's status as non-Checked. The only priority of the player who's King is in check is to eliminate the Check move on the King.
	e)	Check-Mate -> Basically End of Game. This is the same position as Check, but is unable to Uncheck in any number of ways such as: Unable to block with other pieces, unable to move the King, unable to eat pieces that are Checking the King.


### Game-Board
Traditionally 