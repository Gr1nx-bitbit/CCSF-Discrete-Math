# Textbook Reading 3.1
*Inquiry 3.1*: The figure below shows the first three squares in a sequence q0, q1, q2, ... of squares divided into square regions. The next square in the sequence is formed by drawing a “+” inside each region of the previous square. How many nonoverlapping square regions are there in each of the first five squares q1, q2, q3, q4, q5? --> So each time we draw a plus, the square turns into four; if each square turns into four more of itself it looks like a 4^q function but we could also draw it out to make sure

*Inquiry 3.2* Laura is given a starting salary of $2,000 and is promised a 10% raise every month. What will her monthly salaries be for the next three months? --> So when we go to the next month, the current saray is multiplid by 1.1. This means that we multiply by 1.1 over again so it would be 2,000 * (1.1)^n

**So things become recursive when they are defined within terms of themselves**. 

**Ex 3.1** Use Equation 3.1.2 to compute P(5). --> P(5) = [5 + P(4)], P(4) = [4 + P(3)], P(3) = [3 + P(2)], P(2) = [2 + P(1)], P(1) = 1 therefore, 1 + 2 + 3 + 4 + 5 = 15

So just as in CS, we need a non-recursive **base case** so that we'll be able to actually compute something. 

**Definition 3.1** *Fibonacci Numbers* 
F(n) {
    if n == 2 || n == 1 {
        1
    } else if n > 2 {
        F(n - 1) + F(n - 2)
    }
}

Remember: recurrence relations have a **base case** and a **recursive case** which describes a future value based on previous values. 

**Ex 3.4** Let H(n) be the number of circles you need to form a hexagon with n circles on each edge. From Figure 3.3, it is clear that H(2) = 7 and H(3) = 19. Find a recurrence relation for H(n).

H(n) {
    if n = 1 { 
        1
    } else {
        **H(n - 1) +** 6n **- 6**
    }
}

Remember that the height of a binary tree is the amount of edges from the root node to the smallest child. 