# Results

## Colley
   1. 0.868 Florida State      [0] 
   2. 0.751 Clemson            [0]
   3. 0.635 Duke               [+4]
   4. 0.614 Georgia Tech       [-1]
   5. 0.610 Miami              [+1]
   6. 0.581 Virginia Tech      [-1]
   7. 0.505 Syracuse           [+3]
   8. 0.504 Boston College     [0]
   9. 0.468 North Carolina     [-5]
   10. 0.443 Pittsburgh         [-1]
   11. 0.385 Maryland           [+1]
   12. 0.340 Wake Forest        [-1]
   13. 0.149 Virginia           [+1]
   14. 0.146 NC State           [-1]

## Massey

  1. 35.083 Florida State
  2. 16.845 Clemson
  3. 7.126 Georgia Tech 
  4. 2.946 North Carolina 
  5. 2.790 Virginia Tech
  6. 0.764 Miami
  7. 0.408 Duke 
  8. 0.137 Boston College 
  9. -3.514 Pittsburgh
  10. -10.210 Syracuse 
  11. -10.703 Wake Forest 
  12. -11.526 Maryland 
  13. -14.127 NC State 
  14. -16.020 Virginia

## Real Rankings

  1. FSU
  2. Clemson
  3. Boston College
  4. Syracuse
  5. Maryland
  6. Wake Forest
  7. NC State
  8. Duke
  9. Miami
  10. VTech
  11. Georgia Tech
  12. North Carolina
  13. Pitt
  14. UVA

# Conclusions

## Model Comparison

The two models were overall very close to each other - 11 out of the 14 teams in the ACC were ranked in the same position or with a difference of one rank. 
Three teams had a high disparity in their rankings: Duke (4 spots), Syracuse (3 spots), and North Carolina (5 spots). Upon noticing that, I formulated a hypothesis that those teams had won or lost by a high margin. Since Massey's method accounts for differentials and Colley's does not, that would justify the disparities in those rankings. 

Indeed, those three teams had high-differential games that Colley's method would not appropriately adjust for, namely Syracuses's 3 - 59 loss against FSU and their 0 - 56 defeat against GATech, Duke's 7 - 45 defeat against FSU, and North Carolina's 45 - 14 win against UVA. 

Other teams experienced blowout losses, namely Wake Forest's 3 - 59 loss to FSU and their 7 - 56 loss against Clemson, UVA's 10 - 59 loss against Clemson, and Clemson's 14 - 51 loss against FSU. 
There's a reason why that set of games was not as influential: Wake Forest and UVA were very far down in the rankings to begin with, so it is likely that even Massey's model didn't weigh point differentials heavily enough to sink them further than their W/L record already had. Clemson had multiple wins with high point differentials (see previous paragraph) that made their final point differential high. 

## Colley, Massey vs. Real Rankings

The actual rankings are rather far from both predictions. Both models correctly guessed that FSU and Clemson would be 1st and 2nd respectively, but they made severe mistakes in many other estimations. This suggests that there are several factors both models failed to take into account that the actual model used by the ACC to rank teams. Some of them will be discussed below.

## Suggestion 1

There should be a mechanism to account for injured players. E.g. if a team's quarterback was injured and missed a game that was lost, that game should not be weighed as heavily as others to determine the team's ranking. Different players' injuries should have their own different weights.

The weight of each player's injury would be determined by: 

1. The player's performance compared to others playing the same position: their personal rating would be compared to that of the player who replaced them, and the higher the difference is the higher the weight. 
2. How 'critical' their position is (e.g. quarterback > offensive lineman). Each position would have a predetermined weight, and the more critical the player's position the more weight their injury would carry.

This system would at least partially adjust for outcomes that were influenced by a given player's injury. Both teams in the game would be affected by that system - regardless of the outcome, the injured player's team would be benefitted and the team that plays them would be negatively affected. 

## Suggestion 2

The psychological factor of win and loss streaks should be accounted for.

1. If a team is on a win streak, wins should be weighed progressively less heavily. It becomes easier to win when on a win streak, and the longer the streak goes for the less games reflect players' collective psychological strength, which is a crucial factor in determining a team's overall competence.

2. If a team is on a loss streak, a similar logic applies: the longer the streak, the less heavily they will be penalized for another loss. If they get a win, however, that will be more heavily weighted because of how difficult it is to win amidst a long loss streak. 

The value of wins and losses should not start dropping down immediately after a win: there should be a set number of wins or losses after which that would happen. In other words, there would be threshold after which a team is considered to be on a streak rather than the streak starting immediately after a win or loss.

## Suggestion 3

Strength of schedule has to be accounted for. 

When weighing a team's performance, their opponent's ranking in the past season should be considered. The higher their opponent's ranking, the more a win should be weighed and the less a loss should be weighed. The higher the difference between both team's rankings in the conference during the past year, the more heavily the outcome of that game will be weighted for both teams.
