## Results description


There are two files that contain results for the 

- offline case: `offline.json`
- online case: `online.json`

The `offline.json` result file describes in the following sequence:

- for each value of departing area radius $s^r$
- for each value of search radius $R$
- for each value of total number of drivers $N$
- for each scenario BIG, ALL, SMALL
- for each strategy greedy (driver-selfish), self (platform-selfish), VCG (VCG mechanism)
- the following results:	
	- the system cost "total_cost"
	- the individual player's cost "metrics" 
	- the individual player's payement (for VCG) "pricing"
	- the optimal player's cost without any other players in the system "opt_cost" 
	- the difference between the resulting player's cost and the optimal cost
	- the resulting strategy, i.e., which set of stations assigned to each player


The `online.json` result file describes in the following sequence:

- for each value of departing area radius $s^r$
- for the maximal number of drivers possible (here=40)
- for each number of drivers $N$ in the system
- for each value of search radius $R$
- for each scenario BIG, ALL, SMALL
- for each strategy:
	- 0 : VCG-greedy,
	- 1 : VCG-datadriven,
	- 2 : Offline,
	- 3 : Driver selfish,
	- 4 : Platform-selfish
- for strategies 0,1,2:
	- each player's mean cost (utility)
	- each player's mean price 
	- each player's number of drivers
- for strategies 3,4:
	- for each value of elapsed time between two departing driver (0.5, 1.5, 2.5 [min])
	- each player's mean cost (utility, without any prices)




