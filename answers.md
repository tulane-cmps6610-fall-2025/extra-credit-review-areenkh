# CMPS 6610 Extra Credit Answers
  
In this extra credit assignment, we will test and review concepts you
   have learned since the midterm exam. Please add your written answers
   to `answers.md` which you can convert to a PDF using
   `convert.sh`. Alternatively, you may scan and upload written
   answers to a file named `answers.pdf`.



1. **Algorithmic Paradigms**

If I had to choose a favorite algorithm from this unit, I would pick Kruskal’s algorithm. I don’t particularly love any algorithm, but Kruskal’s feels the most intuitive to me. When I do Minimum Spanning Tree problems by hand, Prim’s algorithm can feel mentally overwhelming because I have to keep track of all the edges from all the nodes already included in the tree. In contrast, Kruskal feels more sequential. I simply sort the edges by weight and add the smallest one as long as it doesn’t form a cycle. That step-by-step process feels clearer and less stressful to follow manually, which is why Kruskal’s is the one I prefer.

2. **Divide and Conquer**

Let's assume we are given a set of points and we want to find the closest pair.

If we use divide and conquer:

1. split the set into two 

2. recursively find the closest pair 

This would not be an optimal solution because what if the closest pair has one point in each set. Therefore, a divide and conquer approach would *not* necessarily satisfy the optimal substructure property. 


3. **Randomization**

- 3a. 

We know that $E[Y(n)]<2nln = O(nlogn)$

We can plug this into Markov's inequality 

Let Y(n) be the random number of comparisons quicksort makes on an array of size n. 

This means that: $Y(n)=> cn^2$

This means we want a bound of $P[Y(n) => cn^2]$

Markov's inequality: for any non-negative random variable X and a>0

$P[X=>a]<=E[X]/a$

Take $X=Y(n) and a=cn^2$

$P[Y(n)=>cn^2]<= E[Y(n)]/cn^2 <= 2nln n/cn^2 = 2ln n//cn$

The probability is <= O(logn/n).


- 3b.

4. **Greedy Algorithms**

5. **Dynamic Programming**

6. **Graphs**
