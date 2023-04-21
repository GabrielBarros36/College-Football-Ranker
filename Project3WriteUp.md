# Tasks

## Compare both rankings, distinguish them from one another, write down differences you note.
- Do any teams change in rank by only one position?
- Do any teams change in rank by multiple positions?

## Look up actual 2013 season rankings
- Compare against Colley and Massey rankings

## Measurements
- Think of 3 measurements that you'd think are important for ranking our given dataset

### Notes on Colley's Method

Does NOT take margin of victory into account. 

> point differentials = margin of victory

- First, rank based on Laplace's rule of succession. It uses the winning percentages of every team. 
- Weighs the winning percentage so that it's never 100%, which introduced uncertainty into the system. (there's always the chance of an upset)

### Notes on Massey's Method

- Accounts for point differentials: assumes a difference in rankings provides a predictive point differential for a game.

> The data from games is separated using the matrix equation PR = B

Where P only records wins/losses, R contains the rankings, and B corresponds to the point differentials.

- Method has more equations (games) than unknown variables (teams), so system tends to be inconsistent. Use Least Squares method to find closest possible vector that satisfies the system.

> Final Form:  P<sup>T</sup>PR = P<sup>T</sup>B

term
: definition

# Answers

## Measurements

- Preseason/exhibition games (have to be weighed somehow)
- Injured players if any

# Results

## Colley
   0.868 Florida State      [0] 
   0.751 Clemson            [0]
   0.635 Duke               [+4]
   0.614 Georgia Tech       [-1]
   0.610 Miami              [+1]
   0.581 Virginia Tech      [-1]
   0.505 Syracuse           [+3]
   0.504 Boston College     [0]
   0.468 North Carolina     [-5]
   0.443 Pittsburgh         [-1]
   0.385 Maryland           [+1]
   0.340 Wake Forest        [-1]
   0.149 Virginia           [+1]
   0.146 NC State           [-1]

## Massey

  35.083 Florida State
  16.845 Clemson
   7.126 Georgia Tech 
   2.946 North Carolina 
   2.790 Virginia Tech
   0.764 Miami
   0.408 Duke 
   0.137 Boston College 
  -3.514 Pittsburgh
 -10.210 Syracuse 
 -10.703 Wake Forest 
 -11.526 Maryland 
 -14.127 NC State 
 -16.020 Virginia

## Real Results

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

