# Chess Analysis

## Data Processing
Analysis of which squares in classic chess game are most common to find a king positiones at the  moment of recieving check mates.

Data is processed by filtering games ended by check mate, them splitting games based on the winner ( white or black) and finally extracting all the moves of a single player.
The last operation was conducted in Google sheets using regular expression function.


## Insights

1) There is a clear pattern indicating that right side squares of player are the squares in which proportionally are delivered more check mates. 
2) While border squares contains more checkmates, the % decreases as you move king toward center and left of chess board
3) This is true for both white and black games (when playing as black chess board is reversed, that is why right side of black is on left side of this picture)

![alt text](https://github.com/giandata/check_mates/blob/main/mates.JPG)

4) Further exploration of the games indicated in simmetrically opposite way ti the king's mates how the left-most side of the board is where pawn are mostly promoted.
5) interestingly to discover that column A is the most prolific column for promoting pawns.

![alt text](https://github.com/giandata/check_mates/blob/main/pawns.JPG)

## Conclusion
row and column % are calculated over the total of the games considered therefore are possibly subjected to bias in the case there is disproportion of king / quenn side castling.
However, to find such clear patterns ith Chess data rather then observing more distributed situation, and even assuming bias in the data, it indicates that there is a relation within the 2 findings: when the kings are castled opponent will try to get to mate it perhaps leaving more space on the opposite side of the board, so to allow more pawn to promote.
