# Activities

## Task 1

Refer to the first [link](#links).

- Why is Algorithm Analysis Important?
# Answer: The accidental or unintentional use of an inefficient algorithm can significantly impact system performance
- Explain the Big $O$ notation
# Answer: Big O Notation is a tool used to describe the time complexity of algorithms.
- Compare `Linear`, `Logarithmic`, `Quadratic` and `Constant` complexities.
# Answer:
Name	      Big O
Constant	  O(c)
Linear	    O(n)
Quadratic	  O(n²)
Logarithmic	O(log(n))

## Task2

Refer to the first [link](#links).

- Write a simple algorithm in C++ that finds the square of the first item in a list and then prints it on the screen.

#include <iostream>
#include <vector>

int main() {
  std::vector<int> list = {1, 2, 3, 4, 5};
  int result = list[0] * list[0];
  std::cout << result << std::endl;
  return 0;
}
- What is the complexity of the algorithm?
# Answer: The complexity of the previous algorithm is O(1)

## Task 3

Refer to the first [link](#links).

- Write a simple program that displays all items in a list to the console.
#include <iostream>
#include <vector>

int main() {
  std::vector<int> numbers = {1, 2, 3, 4, 5};
  for (int number : numbers) {
    std::cout << number << std::endl;
  }
  return 0;
}
- What is the complexity of the algorithm?
The complexity of the previous algorithm is O(n), where n is the number of items in the list. This is because the algorithm loops through each item in the list once, and the time it takes to print each item is constant, so the total time taken is proportional to the number of items in the list.


## Task 4: : Individual, at home

Refer to this [pdf](./big_o.pdf):

- What is the difference between complexity and performance:
#  Answer:
Complexity and performance are related but different concepts in big O notation.
    Complexity refers to the upper bound on the growth rate of the running time of an algorithm as a function of the size of its inputs. It provides a theoretical estimate of how the running time of an algorithm will behave as the inputs get larger.
    Performance, on the other hand, refers to the actual running time of an algorithm on specific inputs and a specific implementation on a specific machine. It provides a concrete measure of how long the algorithm takes to run.
So, complexity gives us an idea of how the running time of an algorithm grows as the input size increases, whereas performance gives us a measure of the actual running time of the algorithm for specific inputs and implementation.

- Does complexity affects performance or is it the other way around?
Complexity affects performance, but performance can also affect complexity analysis.
Complexity analysis provides a theoretical estimate of how the running time of an algorithm will behave as the inputs get larger. So, it gives us an idea of how the running time of an algorithm will grow as the input size increases. This information can be useful in choosing the right algorithm for a given problem, as well as in predicting the scalability of an algorithm.
However, the actual running time of an algorithm can be affected by various factors, such as the implementation, the input size, the specific machine it is running on, and so on. These factors can impact the performance of an algorithm, making it either faster or slower than the theoretical estimate provided by its complexity analysis.
So, while complexity analysis provides a theoretical estimate of the running time of an algorithm, it is the performance that gives us a concrete measure of how long the algorithm takes to run.

- Restate the formal definition of big $O$ in plain English

Big O notation is a mathematical way to describe the upper bound of the growth of a function, specifically the longest amount of time it would take to execute an algorithm or solve a problem. It gives an estimation of how fast a function grows as the input size increases, in relation to the worst-case scenario.

## Links

- [Big O Notation and Algorithm Analysis ](https://stackabuse.com/big-o-notation-and-algorithm-analysis-with-python-examples/)
- [Visualization](https://www.cs.usfca.edu/~galles/visualization/Search.html)
- [Big-O notation explained by a self-taught programmer](https://justin.abrah.ms/computer-science/big-o-notation-explained.html)
- [Big-O is easy to calculate, if you know how](https://justin.abrah.ms/computer-science/how-to-calculate-big-o.html)
- https://cpp.sh/
