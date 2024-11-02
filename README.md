# Traveling salesman problem

The aim of this code is to solve the TSP problem.

### Greedy
The greedy algorithm starts from a city and hops to the closest city. There's also a parameter to adjust the probability to hop to the second, third, etc., closest city, which can produce better results.

### Evolutionary
The initial population is composed of several solutions produced with the greedy approach. I've tried several alternatives for the mutation, and `inversion mutation` is the only one that actually works. Different types of crossover don't influence the final result much, but it seems that `cycle crossover` performs better on average. I've run the algorithm multiple times and selected the best performing one.

### Results
#### Best paths
![TSP Vanuatu](./images/TSP_vanuatu.png)
![TSP Italy](./images/TSP_italy.png)
![TSP Russia](./images/TSP_russia.png)
![TSP US](./images/TSP_us.png)
![TSP China](./images/TSP_china.png)

#### Fitness evolution
![Fitness Evolution Vanuatu](./images/fitness_vanuatu.png)
![Fitness Evolution Italy](./images/fitness_italy.png)
![Fitness Evolution Russia](./images/fitness_russia.png)
![Fitness Evolution US](./images/fitness_us.png)
![Fitness Evolution China](./images/fitness_china.png)
