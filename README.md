# PROHACK-2020
My solution to PROHACK the International Data Science Hackathon by McKinsey &amp; Company with a public leaderboard score: 0.03050063 &
private leaderboard score: 0.03671962

![cover photo](Cover%20Photo.jpg)

## Challenge
An advanced intergalactic species have reached the highest levels of development, almost achieving singularity. They consume energy measured in DSML units and live widespread across different star clusters and galaxies. They need to optimize their well-being across all those galaxies; They have a lot of data, and they want humans to help.
Only two steps prevent them from achieving singularity:
1. **To understand what makes them better off**

Using the data, train a model to predict the well-being index with the highest possible level of certainty.

2. **To achieve the highest possible level of well-being through optimized allocation of additional energy**

Having discovered a star of unusually high energy of 50000 zillion DSML, what is the optimal distribution given that:
* No one galaxy will consume more than 100 zillion DSML
* At least 10% of the total energy will be consumed by galaxies in need with existence expectancy index below 0.7
* Every galaxy has a certain limited potential for improvement in the Index described by the following function: 
**Potential for increase in the Index = -np.log(Index+0.01)+3**
* Likely index increase dependent on potential for improvement and extra energy availability is described by the following function:
**Likely increase in the Index  = extra energy * Potential for increase in the Index ^2 / 1000**


## Evaluation
Solutions are evaluated on two criteria: 
1. Predicted future index values evaluated using RSME metric
2. Allocated energy from the newly discovered star evaluated using RSME

Leaderboard Score: 80% prediction task RSME + 20% optimization task RSME * lamda (where lambda is a normalizing factor)

Leaderboard is 80% public and 20% private
