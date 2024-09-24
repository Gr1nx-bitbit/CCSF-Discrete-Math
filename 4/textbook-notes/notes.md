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
The **degree** of a vertex is the number of times an edge touches it (not just how many individual edges touch it); an edge can touch a vertex multiple times via loops. **Indegrees** are how many edges connected to the vertex that lead into it, while **outdegrees** are the opposite. A **path** is the sequence of verticies connected by edges where the ith edge connects the ith-minus-one vertex and the ith vertex. A **circuit** is a graph whose end vertex is the same as its start vertex. Graphs are **connected** if any two or more verticies are connected. 

In graphs, the degree number is twice that of the edge number (since edges connect two verticies). 

### Modeling Relationships with Graphs
The **coloring** of a graph is when you assign metadata to a vertex (metadata can be shared between vertecies) i.e. two vertecies can have a "color" or value of "323 elephants" or something else arbitrary. A graph is **planar** if you cna draw it without any of the edges crossing each other. A graph with numerical values (**weights**) on its edges is called a **network**.

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
