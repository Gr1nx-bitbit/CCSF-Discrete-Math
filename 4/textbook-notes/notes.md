    - This chapter is about figuring out and defining relationships between different *sets* of data. Can be shown as *graphs*.
# Textbook Reading 2.1: Graphs
Graphs are the mathmateical way of drawing relationships between discrete sets of data. 
*Inquiry 2.1*
- a: Draw a diagram that shows the natural numbers 3, 4, 5, 6, 7, 8 and indicates which pairs of numbers are relatively prime. Include instructions that explain how to interpret your diagram.
    - Insert PDF
- b: If two natural numbers are relatively prime to a third, must they be relatively prime to each other? Prove or disprove.
    - Answer: This is false since 4 and 7 are connected, and 7 is connected to 6. 4 and 6 are both divisible by 2. 
- c: an you separate the numbers 3, 4, 5, 6, 7, 8 into groups such that each group consists of numbers that are relatively prime to each other? What is the fewest number of groups required? Explain how you know.
    - The node 4 group and node 6 group contain the least relative primes since those nodes have the least edges.

*Inquiry 2.2*
- a && b: Sketch a simple diagram showing the countries Russia, Estonia, Latvia, Lithuania, Belarus, Ukraine, and Poland. Your diagram should show which countries border each other, but otherwise it should be as simple as possible. && Is it possible to plan a round trip (on land) through all these countries that visits each country exactly once? Is there more than one way to plan such a trip?
    - Insert PDF
- c: How many pairs of these countries share a border? Is it possible to plan a trip through all these countries that visits each border crossing exactly once? Find one, or explain why it is impossible.
    - I don't really understand the question

### Edges and Verticies
Nodes are the **verticies** and the connecting lines between nodes are **edges**. Directed graphs have arrows on the edges while undirected graphs don't. 

### Terminology
The **degree** of a vertex is the number of times an edge touches it (not just how many individual edges touch it); an edge can touch a vertex multiple times via loops (really its how many edges branch out from the vertex!). **Indegrees** are how many edges connected to the vertex that lead into it, while **outdegrees** are the opposite. A **path** is the sequence of verticies connected by edges where the ith edge connects the ith-minus-one vertex and the ith vertex. A **circuit** is a graph whose end vertex is the same as its start vertex. Graphs are **connected** if any two or more verticies are connected. 

In graphs, the degree number is twice that of the edge number (since edges connect two verticies). 

### Modeling Relationships with Graphs
The **coloring** of a graph is when you assign metadata to a vertex (metadata can be shared between vertecies) i.e. two vertecies can have a "color" or value of "323 elephants" or something else arbitrary. A graph is **planar** if you cna draw it without any of the edges crossing each other. A graph with numerical values (**weights**) on its edges is called a **network**. An **Euler Path** is one in which every edge is used exactly ONCE. 

Example 2.3: Several departments around campus have wireless access points (WAPs), but problems arise if two WAPs within 200 feet of each other are operating on the same frequency. Suppose the departments with WAPs are situated as follows.

|Department|Is within 200ft of other departments|
|:--------:|:----------------------------------:|
|Math|Physics, Psychology, Chemistry, Sociology|
|Sociology|History, English, Economics, Math, Chemistry, Psychology|
|Physics|Math, Chemistry|
|Psychology|Math, Chemistry, Sociology, Economics|
|History|Sociology, English|
|English|Economics, Sociology, History|
|Economics|English, Sociology, Psychology|
|Chemistry|Math, Psychology, Sociology, Physics|

Solution attempt: We're going to need as many frequencies as as the vertex with the most edges, I think. There might be a problem if that vertex shares an edge with another vertex that has n - 1 frquences. I got it right I think. 

# Textbook Reading 2.2: Sets
*Inquiry 2.3*: A certain discrete mathematics class consists of 21 students. Of these, 10 plan to major in mathematics and 13 plan to major in computer science. Five students are not planning to major in either subject. How many students plan to major in both subjects? Draw
a diagram to explain your reasoning.
- I can kind of visualize venn diagrams but it feels like there could be a lot of variability, like 11 students can be majoring in BOTH CS and Maths leaving only 2 other students to major in CS. We do know that 5 students won't major in either which leaves us with 16 students in total majoring in either CS, Maths, or both. From there we can only guess though or come up with a set of possibilites (haha, get it?). 

*Inquiry 2.4*: Explain the distinction between the following two scenarios.
- Scenario A: A professor chooses three students to work together on a problem.
    - 3 unique students 
    - One common problem
- Scenario B: A professor asks three questions in sequence, and each time calls on a student to answer.
    - 3 unique problems
    - common body of students (duplicates possible)
- How are the professor’s choices constrained in each scenario? Compare and contrast.
    - In the first scenario, the professor needs to pick 3 unique students to work on a singular problem while in the second scenario the professor is constrained to 3 problems and has to pair a student to each answer; the student for each answer can be any of the available ones i.e. they don't have to be unique.

*Inquiry 2.5*: Consider the following collections of natural numbers.
- Collection T: All multiples of 2.
- Collection R: All multiples of 3.
- Collection S: All multiples of 5.
- How are these collections related? Is there any overlap? Explain your findings in some organized way.
    - Numbers in each collection can appear in a different collection. 

A way of desribing *related groups of objects* is through **sets**. Something can be said to be in a set like when defining functions, f(x) = 2x + 3, x ∈ *S*. Or we can show what a set defines like so: *S* = {x1, x2, x3, ..., xn}. We can also say that certain elements of the set have a property; this can be denoted using the pipe (| but it's called "set builder notation") --> {x ∈ S | x has property p}. We can also make new sets from old sets like so:
- Initial set: A = {1, 2, 3, 4, 5, 6, 7, 8}
- New set: B = {x ∈ A | x is odd} => B = {1, 3, 5, 7}
There are also common/colloquial sets like **Z** for all positive integers, **N** for all natural numbers, and **R** for all real numbers. 
There is a common symbol used for the predicate logic of (Vx)(x ∈ A -> x ∈ B) --> A ⊆ B [⊆ is the set equivalent for ->], or A is a subset of B. Ø is another special set which is the *empty set*; that is, there are no elements in it therefore it is a subset of every set. The *union* of sets is a set where all the elements of its components are contained i.e. (Vx)(A ∪ B) is equivalent to (Vx)([x ∈ A] v [x ∈ B]) --> A ∪ B = {x | (x ∈ A) v (x ∈ B)} and consequently (Vx)[x ∈ A ∪ B <--> (x ∈ A) v (x ∈ B)]. ∩ is set AND equivalent, so C = A ∩ B means that C is a set that contains the elemts that A and B have in common. A ∩ B = {x | (x ∈ A) ^ (x ∈ B)}. The domain is implicit which is really the *Universal set*. The **complement of a set** is all elements in the Universal set expect the ones in the original set e.g. A = {...}, A' = {x ∈ U | x ∉ A} OR A' = {x ∈ U | ¬(x ∈ A)}. To say two sets are equal we use <--> or =. A = B is equivalent to (Vx)(x ∈ A <--> x ∈ B). 

I need to go back over the proofs man...

The *power set* is the set that holds all the subsets of another set --> P(S) = {X | X ⊆ S}
Sets may have different types of elements; some sets' elements will be numbers, others, tuples, others sets, etc. 

p => p v q == A ⊆ (A ∪ B), De Morgan's laws --> (A ∪ B)' = A' ∩ B' --> (A ∩ B)' = A' ∪ B'. 

### Identities
Just like how we proved stuff using propositional logic, we can do the same with set theory. If a set has a finite number of items in it, we can represent that by using the absolute value notation. If *S* is the set that holds the members of the House of Reps, then |*S*| = 435. You can then use set magnitudes as numbers in an equation e.g. a student society has 11 members, 8 of which have 2400 SAT scores and 5 of which have 4.0 GPAs; how many members have both 2400 SAT and 4.0 GPAs? --> A = {x | x is a student with 4.0 GPA}, B = {x | x is a student with a 2400 SAT score} 11 = 8 + 5 - |A ∩ B| --> |A ∩ B| = 13 - 11 --> |A ∩ B| = 2, therefore there are two students how have both 2400 SAT scores and 4.0 GPAs. 