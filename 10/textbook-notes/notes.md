# Reading 4.1: Basic Counting Techniques
A **disjoint set** is one in which the union of two sets = Ø - usually either or type stuff. 

**Theorem 4.1** Suppose A1, A2, ..., An are pairwise disjoint sets, that is Ai ≠ Aj for all i and j with i ≠ j. Then A1∪A2∪...∪An = |A1| + |A2| + |...| + |An|. -- Proved by induction. 

<font color="green">We can always think of a Cartesian prodct A x B as a grid!</font>. The number of elements (ordered pairs) in a cross product of sets is |A|•|B|. You can represent cross products as trees - the root node is just a starting point then the children of the root are the elements in one of the sets and the children of the root's children are the elements in the second set - can be expanded to an n cross prodcut. 

**Theorem 4.2** Suppose A1, A2, ..., An are finite sets, then A1 x A2 x ... x An = |A1|•|A2|•|...|•|An|

# Reading 4.2: Selections and Arrangements
Selections have to do with selecting a subset of elements from a set while arrangements have to do with selecting elements and then arranging them in some order. The **arangement principle** which has its roots in multiplication is *the number of ways to form an **ordered** list of r distinct elements drawn from a set of n elements by* --> P(n, r) = (n!)/(n - r)! - These are called **permutations**. <font color="green">The **selection principle** is different because it deals with unordered sets.</font> The selection principle tells us how many ways to choose a subset of r elements from a set of n elements is --> C(n, r) = (n!)/r!(n - r)! - Also C(n, k) = C(n, n - k). Another good thing to know is that we can expand (a + b)^n in a simpler way:

**Theorem 4.3**: Let j and k be non-negative integers such that j + k = n. The coefficient of the aj bk
term in the expansion of (a + b)n is C(n, j).