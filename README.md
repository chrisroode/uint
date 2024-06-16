# uint
Open Source, Crowd Sourced table top game with the goal of making computer science a cool thing you would buy at Target.

## Getting started.
There's barely anything here, but soon there will be the mechanics for the game.  See the following subfolders for different aspects of the package.  Outline below:

### book
The intended game will ship with a rule book of types.  Each two page spread of the book contains different games that can be played with the uint cards.  Games can be designed for solitare play, two players, or 3-4 players.  Also, considering the complexity of algorithms presented in the game, the game can be played in teams for more experienced players to assist beginners.

### cards
The main feature of the game is the deck of cards.  A simple design that is symmetrical (like regular playing cards).  These cards however, contain the three representations of a number:
	- decimal
	- hexidecimal
	- binary
A deck would comprise of a set of unsigned integers ranging from 0-255.  This would allow shuffling and dealing in the max capacity allowing each player to have 64 cards to work with.

### marbles
The larger game setup would consist of a random access memory array represented with marbles that can be placed on an 8x8 grid of dimples.  The exact use configuration of the memory array would be unspecified and can change based on the specific game.

Marbles would come in three colors, and could represent up to 2 bits of information if the game required.
	- 0b00: absence of a marble
	- 0b01: represented by a Black marble.
	- 0b10: represented by a White marble.
	- 0b11: represented by a Purple, specifically Milly Bobby Brown's favorite color.
		Reference: Milly Bobby Brown is the actress who plays Eleven from Stranger Things.
		https://youtu.be/PqGehRgKTLo?si=QGqXjtywT3bJMYD0&t=237

The total memory allowed with this representation would be 256 bits of RAM.  Disregarding color, 64 bits would be more practical in larger group settings.

### push pop bubbles
For a travel edition, the marble memory could be represented using push pop bubbles.  Current market research shows that they already are easily available in 3x3 and 4x4 grids.  However, for a computer representation, either a 4x4 or 4x8 grid would be more ideal.  For prototyping, this will not need to be used.

# Game configurations
The main setup for the game:
Of course, the solitare and two player games can be arranged however the player would like.  Things get tricky for two or more players.  The book would help with this.

To assist with more complicated games, the instruction set would be organized in a grid, and post-it arrow flags would be provided so players can keep track of where they are in the game.  Therefore, two two player games would need two copies of the instructions on one spread.  This would allow two players to sit side by side and keep track of their own set of rules.

For larger games, involving 4 players, a supplemental book would provide additional copies of the rules for the multi player games.  This way four players could set up across from each other and play together without having to struggle to see the algorithms.



## Three sizes of configurations.
Plan for three scales of game configuration.

### uint - The Whole Byte
Large table top box set.  Includes:
- 1 deck of 256 cards, numbered 0x00 -0xff.
- four 8x8 marble grids.
- 1 triple marble bin (for sorting colors)
- a plentiful supply of marbles TBD in the colors mentioned above.
- A large spiral bound booklet with games and rules.
- A thinner spiral bound book with supplemental copies of instructions for the 3-4 player games..to assist with playing stations.
- A set of post-it arrow flags to act as an instruction counter.

### uint - x64 edition
A smaller travel edition.
- 1 deck of 64 cards: 0x00 - 0x40
- Two push pop bubble memory blocks.
- A small size booklet (spiral bound) with games.

### uint - just a nibble.
A package that fits the dimensions of a standard deck of cards, only thicker.
- a deck of cards containing for sets of 0x0 - 0xF.  They would be colored to be different 'suits'
- a miniature booklet containing various games that can be played.


# Dependencies:
- The font specified for the playing cards is JetBrains Mono.
- Font specified for booklet design is Open Sans.