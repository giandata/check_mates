# Chess Analysis

Analysis of which squares in classic chess game are most common to find a king positiones at the  moment of recieving check mates.

Data is processed by filtering games ended by check mate, them splitting games based on the winner ( white or black) and finally extracting all the moves of a single player.
The last operation was conducted in Google sheets using regular expression function.


# Insight

1) There is a clear pattern indicating that right side squares of player are the squares in which proportionally are delivered more check mates. 


2) Further exploration of the games indicated in simmetrically opposite way how the left-most side of the board is where pawn are mostly promoted.
