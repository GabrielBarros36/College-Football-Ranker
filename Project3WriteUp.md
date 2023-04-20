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

> Final Form: P^2^ PR = P ^T^ B

term
: definition
