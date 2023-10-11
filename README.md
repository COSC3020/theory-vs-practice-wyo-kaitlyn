[![Open in Visual Studio Code](https://classroom.github.com/assets/open-in-vscode-718a45dd9cf7e7f842a935f5ebbe5719a5e09af4491e668f4dbf3b35d5cca122.svg)](https://classroom.github.com/online_ide?assignment_repo_id=12055559&assignment_repo_type=AssignmentRepo)
# Theory vs. Practice

- List 3 reasons why asymptotic analysis may be misleading with respect to
  actual performance in practice.

  1. Analysis ignores constants
  2. Only true until you reach a certain input size
  3. The analysis can sometimes not be representatitve of how the algorithm actually grows
  in practice - $\Omega$(1) will be true for everything, but that won't actually tell
  you anything about the algorithm

- Suppose finding a particular element in a binary search tree with 1,000
  elements takes 5 seconds. Given what you know about the asymptotic complexity
  of search in a binary search tree, how long would you guess finding the same
  element in a search tree with 10,000 elements takes? Explain your reasoning.

  $T(n) \leq c f(n) \forall n \geq n_0$
  
  $5 s = c\log_2 1000$
  
  $1/2 s = c$

  $T(n) = \frac{1}{2} \log_2 10000$
 
  $T(n) = 6.64 s$
  
- You measure the time with 10,000 elements and it takes 100 seconds! List 3
  reasons why this could be the case, given that reasoning with the asymptotic
  complexity suggests a different time.

  1. Hardware - could have run the program on a computer that did not have much
  processing power
  2. Other processes in background could have effected run time by diverting
  resources away from the program
  3. Analysis assumes all operations take same amount of time - the program could
  include operations that taken longer to operate

Add your answers to this markdown file.
