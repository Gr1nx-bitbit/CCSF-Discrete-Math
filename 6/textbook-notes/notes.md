## Textbook Reading 2.5
*Inquiry 2.13*: A round robin is a type of tournament in which each participant plays every other participant exactly once. In a sport without ties (e.g., tennis), will a round robin always produce a clear tournament champion? Justify your answer with examples. --> I think there'ew really only two cases we have to look at: even and odd. If we're in an even case let's say we have 4 people competing, 1 will compete with 2 and 3 will compete with 4; 1 and 4 win and then they go against each other and 4 wins. 1 hasn't played against 3 and 2 hasn't played against 4; 3 wins and then 4 wins, so 3 and 4 have to go at it again. Everyone has played each other exactly once but we still don't have a winner yet since 3 and 4 still have to compete. If we have 3 people compete, let's say 1 plays against 2. 1 wins, so 2 and 3 have to play against each other; 3 wins so 1 and 3 have to play, 3 wins and each player has played against every other player once and we have 1 winner.

**Definition 2.10** A relation *R* on a set S is a **partial ordering** if it satisfies all three of the
following properties.
- a. Reflexivity. For any a ∈ S, a *R* a.
- b. Transitivity. For any a, b, c ∈ S, if a *R* b and b *R* c, then a *R* c.
- c. Antisymmetry. For any a, b ∈ S, if a *R* b and b *R* a, then a = b.

With proving partial orderings, you have to prove each property. One example of a partial ordering is the ≤ operator, however **≤** is used as a **generic partial ordering**. If that operator is used on a set to give it a partial ordering then you can say (S, ≤) is a partially ordered set or *poset* for short. It's possible to have elements in a set that neither a ≤ b nor b ≤ a; these elements are called **incomparable**. If a set has no incomparable elements it's said to have a **total ordering**. **Hasse diagrams** describe sets via a heirarchical graph. Each element in a partially ordered set is called a node and the we use **un**directed edges to show hierarchies i.e. a node will have an undirected edge from it to another node if x ≤ y. We can have **minimums and maximums**; minimums are defined by *m*, x ∈ X (m ≠ x), no such x ≤ m; maximums are defined as *M*, x ∈ X (M ≠ x), no such M ≤ x. 

An example of a partially ordered set would be the set of tasks (T) you have to do in a day such as getting dressed. (T, ≤) with x and y being tasks, x ≤ y signifies that task x must be done before task y. However soem tasks don't depend on others which will prevent one from having a totally ordered set. If you want to make a total ordering, then you need to decide on a sequence and make sure the total ordering is compatibale with the partial ordering, formally meaning, x ≤ y => x ≤sub-t y for all x, y ∈ T. This is known as **topological sorting** which involves making an ordered list of T. Start with minimal element and branch up to maximal elements until you have a tree kinda thing. An **isomorphism** is a map (tree) that describes similarity between structures of problems.

We can also have two sets that are partially ordered (X, ≤1) and (Y, ≤2) that can have a one to one correspondence, that is f: X -> Y, a ≤1 b = f(a) ≤2 f(b) for all a, b ∈ X. Then f is an isomorphism and we write (X, ≤1) ≅ (Y, ≤2). 

**Theorem 2.3** Let q = (p1)(p2)(...)(pn) be the product of the first n primes, and let F ⊆ N be the set of all factors of q. Then (F, |) ≅ (P({1, 2, ..., n}), ⊆).

**Boolean algebra** is our connection between propositional logic and posets. If we have (X, ≤) for any a, b, ∈ X we define the **meet** of these elements (a ^ b) to be the greatest lower bound of a and b. Formally a ^ b is defined by the properties:
- a ^ b ≤ a and a ^ b ≤ b
- if some x ∈ X, x ≤ a and x ≤ b then x ≤ a ^ b; in english that might sounds like, if x is a task before a and x is a task before b, then x is a task before a AND b. 
Formally, the **join** of two elements would have the properties:
- a ≤ a v b and b ≤ a v b
- if some x ∈ X, a ≤ x and b ≤ x, then a v b ≤ x
If every pair of elements have a meet and a join, then they are called a **lattice**. 
Lattices must satisfy these properties:
- Commutativity: a ^ b = b ^ a and a v b = b v a
- Associativity: a v (b v c) = (a v b) v c and a ^ (b ^ c) = (a ^ b) ^ c
- Absorption: a v (a ^ b) = a and a ^ (a v b) = a
Three more porperties for a lattice to become a **boolean algebra** on 149. 

**Theorem 2.4** Let X be a finite set. Suppose that the poset (X, ≤) is a Boolean algebra. Then |X| = 2^n for some n ∈ N, and:
    (X, ≤) ≅ (P({1, 2, ..., n}), ⊆).