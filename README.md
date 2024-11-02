# Traveling salesman problem

The aim of this code is to solve the TSP problem.

### Greedy
The greedy I used starts from a city and hops to the closest city. There's also a parameter to adjust the probability to hop to the second, third etc. closest city, which can produce better results.

### Evolutionary
The initial population is composed of several solutions produced with the greedy approach.
I've tried several alternatives for the mutation and `inversion mutation` is the only one that actually works.
Different types of crossover don't influence much the final result, but it seems that `cycle crossover` performs better on average.
I've run the algorithm multiple times and selected the best performing one.

### Results
#### Best paths
<div style="display: flex; flex-wrap: wrap; justify-content: space-around; gap: 10px;">
    <img src="./images/tsp_vanuatu.png" style=" max-width: 100%; max-height: 100%;" alt="TSP Vanuatu">
    <img src="./images/tsp_italy.png" style=" max-width: 100%; max-height: 100%;" alt="TSP Italy">
    <img src="./images/tsp_russia.png" style=" max-width: 100%; max-height: 100%;" alt="TSP Russia">
    <img src="./images/tsp_us.png" style=" max-width: 100%; max-height: 100%;" alt="TSP US">
    <img src="./images/tsp_china.png" style=" max-width: 100%; max-height: 100%;" alt="TSP China">
</div>

#### Fitness evolution
<div style="display: flex; flex-wrap: wrap; justify-content: space-around; gap: 10px; margin-top: 20px;">
    <img src="./images/fitness_vanuatu.png" style="max-width: 100%;" alt="Fitness Evolution Vanuatu">
    <img src="./images/fitness_italy.png" style="max-width: 100%;" alt="Fitness Evolution Italy">
    <img src="./images/fitness_russia.png" style="max-width: 100%;" alt="Fitness Evolution Russia">
    <img src="./images/fitness_us.png" style="max-width: 100%;" alt="Fitness Evolution US">
    <img src="./images/fitness_china.png" style="max-width: 100%;" alt="Fitness Evolution China">
</div>