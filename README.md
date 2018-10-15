# SimulatedAnnealing
Implementation of the Simulated Annealing Algorithm in solving the (Symmetric) Travelling Salesman Problem. 

In the outer loop of our algorithm, we reduce T by setting T =  0.9 $ \times $ T. While, in the inner loop, we obtain * L * different solutions at each T. These solutions are generated by randomly swapping two indexs(cities) of tour x. 

Then we apply the Metropolis acceptance Probability=min $ \{1, exp(-(fy-fx)/T)\} $ as the probability of accepting a new possible solution. The algorithm then repeats while T > $\epsilon$, with $\epsilon$ = $10^{-2}$,  and stops otherwise.
