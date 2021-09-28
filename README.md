# Chess Analysis

## Data Processing
Analysis of which squares in classic chess game are most common to find king at the moment of receiving check mate.
Over 20000 games are analyzed and 2476 ended by check mate.

Data is processed by filtering games ended by check mate, then splitting games based on the winner (white or black) and finally extracting all the moves of a single player.
The last operation was conducted in Google sheets using regular expression function.
Finally the 2 dataset are joined together for a single visualization.

## Insights

1) There is a clear pattern indicating that right-side squares of the board are the squares in which proportionally are delivered more check mates, where H8 square (black king short castling derived) is the square where most mates are delivered. 
2) While border squares contains more checkmates, the % decreases as you move king toward center and left of chess board.
3) This is true for both white and black games (when playing as black chess board is reversed, that is why right side of black is on left side of this picture)

![alt text](https://github.com/giandata/check_mates/blob/main/mates.JPG)

4) Further exploration of the games indicated in simmetrically opposite way ti the king's mates how the left-most side of the board is where pawn are mostly promoted.
5) It is interesting  to discover that column A is the most prolific column for promoting pawns.

![alt text](https://github.com/giandata/check_mates/blob/main/pawns.JPG)

## Conclusions
Both row and column % are calculated over the total of the games considered therefore are possibly subjected to bias in the case there is disproportion of king / queen side castling.
However, to find such clear patterns in chess data rather then observing more distributed situation, and even assuming bias in the data, it indicates that there is a relation within the 2 findings: when the kings are castled opponent will try to get to mate it perhaps leaving more space on the opposite side of the board, so to allow more pawn to promote on the opposite side.
