## Textbook Reading 2.3
**Functions** are relatinoships between two or more sets of objects where the value of at least one object is completely dependent on another (think about parametric equations). 

**Definiton 2.1**: An f-graph is a directed graph where each vertex has outdegree 1.

*Inquiry 2.6* Give an example of an f-graph with at least five vertices. Invent a shorthand notation that encodes all the information needed to reconstruct the graph. --> f(x) = x^2 + 1 {0 < x ≤ 5}

*Inquiry 2.7* An f -graph is called epi if each vertex has indegree 1. Give an example of an epi f -graph and an example of a non-epi f -graph. Make some conjectures about the properties of epi f -graphs. Can you prove them? --> So, important to remember, just because the definition says an f-graph's vertecies have one outdegree does NOT mean they can't have indegrees. So then, by an indegree, I think they mean that the value of the function set is the same as the origin set; therefore I think an epi f-graph would be something like f(x) = x.

*Inquiry 2.8* Let E be the set of even integers and let O be the set of odd integers. Suppose that a computer is programmed to input a sequence of elements of E and output a sequence of elements of O according to some rule. You run a test of this program using 12, 6, 8, 10, 2 as input, and the computer outputs 81, 9, 25, 49, 1. What rule does the computer appear to be using? --> 12 goes to 81, 6 goes to 9, 8 goes to 25, 10 goes to 49, 2 goes to 1. It seems like 1 is being subtracted; idk

**Definition 2.2**: A function from a set X to a set Y is a well-defined rule that assigns a single element of Y to each element of X. If f is such a function, we write: f : X -> Y, and we denote the element of Y assigned to x ∈ X by f (x). The set X is called the domain of the function, and the set Y is called the codomain. --> Ok, so this means that each element of X has one value of y but doesn't necessarily mean that all numbers in the set of Y will be used up, as an example think of x^2, the set Y is **R** but only a fraction of those numbers are used. 

Functions can also be called **maps**; like a thing that defines the route from one value in a set to another. 

Ex 2.21 Let N = {−2,−1,0,1,2}. Define a function s: N → N by s(n) =n^2 −2. Represent this function with a directed graph.
This seems a bit weird; we know what the set of N is but we also know that an f-graph needs to have every value of x point to a value of y. Does that mean this isn't an f-graph because we can only square -1, 0, and 1 to stay in the set. Nevermind, I didn't see the -2 lol.

A **well-defined** function means that there is an f(x) value for every x in the domain. You can fail to have a well defined function if an x value doesn't have a y value or if the same value ambiguously maps to more than one output value. Make sure that when you're defining a function on a domain to try and confirm its well-defined. Proofs are weird dude. 

**Definition 2.3** A function f : X → Y is injective (or one-to-one) if, for all a and b in X, f (a) = f (b) implies that a = b. In this case we say that f is a one-to-one mapping from X to Y. --> Basically only one value of x can map to its output; there are no output values can be repeated!

**Definition 2.4** A function f : X → Y is surjective (or onto) if, for all y ∈ Y, there exists an x ∈ X such that f (x) = y. In this case we say that f maps X onto Y. --> every element in the set of Y is mapped to, regardless of duplicates; multiple x's can map to a single y (x^2).

An **image** is a way of describing the set of all values a function can take on i.e. shows the relationship between the X set and the Y set via directed edges. 

**Ex 2.26** Prove that the function f : Z → Z defined by f (x) = 2x + 1 is one-to-one. --> so we need to show that each x only maps to a single y. So if we suppose the opposite to be true and prove something that's false that would be cool. How do you show something to be one-to-one?? Ahh, so they used the defintion for a one-to-one showing that if f(a) equals f(b), then a has to equal b. 

**Ex 2.27** Let f : R→ Z be defined by f (x) = ⌊x⌋. Prove that f maps R onto Z. Ah, ok, so we know ⌊x⌋ ∈ **R** and that Z ⊆ **R**, therefore ⌊x⌋ maps onto Z. Ok, so I got it right for the most part except we are saying that n ∈ Z and that Z ⊆ **R** so n ∈ **R** as well. 

A function that is both one-to-one and onto is called a *one-to-one correspondence* or a *bijection*. 

**Ex 2.28** Prove that the function f : R → R defined by f (x) = 2x + 1 is a one-to-one correspondence. Ok, so to prove the onto part, we have to take a value from 2x + 1 and show that it comes from some x; 2x + 1 ∈ **R** and x ∈ **R** therefore the function is onto. Now to prove that the function is one to one; 2a + 1 = 2b + 1 -> 2a = 2b -> a = b therefore one y value can only come from a single x value. Ehh, idk if this is right, the book did it some other way.

We can create new functions by composing old ones (f ◦ g); f ◦ g does not necessarily equal g ◦ f. Undoing a function to map a value back to where it came from is called the inverse. Inverse functions have to be one-to-one and there is a semi-example on 121. I have no idea what the last part is about.

An **inverse function** is one that undos an orginal function; basically it maps the codomain elements back to the original domain elements.

## Textbook Reading 2.4
A **relational** is a more general mathmateical object that describes relationships. 

**Definition 2.5** An r-graph is a directed graph with no multiple edges. That is, for all vertices u, v, there can be at most one edge from u to v.

*Inquiry 2.9* Recall Definition 2.1. Is every f-graph also an r-graph? Explain. --> It seems like it; an f-graph's domain elements have at most one outdegree but that doesn't necessarily mean that all the codomain elements have 1 indegree or an indegree at all; aha, so not all because some of the verticies might not have edges connecting them; does that actually violate the definiton? Oh, EACH vertex has one outegree therefore u can have an edge towards v and v can have an edge towards u.

*Inquiry 2.10* Give an example of an r-graph with at least five vertices that is not an f-graph. Invent a shorthand notation that encodes all the information needed to reconstruct the graph. Compare to Inquiry Problem 2.6. --> A one to one graph i think?

*Inquiry 2.11* Construct a directed graph whose vertices represent the integers 1, 2, ..., 7, where there is an edge from vertex n to vertex m if m − n is even. What properties do you notice about this graph? Would these properties remain if the graph were constructed using a longer list of integers? --> Nah

**Definition 2.6** A relation on a set S is a subset of S × S. If R is a relation on S, we say that “a is related to b” if (a, b) ∈ R, which we sometimes write as a R b. If (a, b) ∉ R, then a is not related to b; in symbols, a /R b.

**Ex 2.34** If S = {1, 2, 3} and the symbols =, <, >, ≤, ≥ all define relationships on Z then the relation of S defined by < is {(1, 2), (1, 3), (2, 3)}

If a, b, ∈ P and a *R* b means that a and b are brothers, then R is a relationship on P. We can also define relationships like so:
Let W be the set of all web pages; L = {(a, b) ∈ W x W | a has a link to b}, then (a, b) means the web page a in the first W has a link to the web page B in the second W. 

**Definition of modulus (≡ n)** is x = a + kn

**Definition 2.7** Let *R* be a relation on a set X. The directed graph associated with (X, *R*) is the graph whose vertices correspond to the elements of X, with a directed edge from vertex x to vertex y whenever x *R* y.

**Symmetric relations** are ones where a *R* b is true (a has a directed edge to b) and b *R* a is also true. 

**Definition 2.8** Let *R* be a relation on a set X, and suppose x *R* y ⇔ y *R* x for all x, y ∈ X. The undirected graph associated with (X, *R*) is the graph whose vertices correspond to the elements of X, with an (undirected) edge joining any two vertices x and y for which x *R* y.

The strict definition of a relationship is that each element in the domain has an outdegree towards another element. The difference between relations and functions is that function outputs depend on their respective inputs while relationships cam be had between however many or few elements. By the way, the '|' sign is a modulo operator where a | b means a modulos b, 2 | 6 = 0 because 6 % 2 = 0. 

**Definition 2.9** A relation *R* on a set S is an equivalence relation if it satisfies all three of the
following properties.
1. *Reflexivity*. For any a ∈ S, a R a.
2. *Symmetry*. For any a, b ∈ S,a *R* b ⇔ b *R* a.
3. *Transitivity*. For any a, b, c ∈ S, if a *R* b and b *R* c, then a *R* c.

For proofs using definiton 2.9, you have to prove each property! Look at examples 2.42 and 2.43. **Partitions** are distinct blocks within sets; the set P = {X, Y, Z} is a partition of S; X ∩ Y = Ø && Y ∩ Z = Ø

**Theorem 2.2** Let *R* be an equivalence relation on a set S. For any element x ∈ S, define R(sub-x) = {a ∈ X | x *R* a}, the set of all elements related to x. Let P be the collection of distinct subsets of S formed in this way, that is, P = {R(sub-x) |x ∈ S}.Then P is a partition of S.

**Proposition 2.1** Let [a] and [b] be equivalence classes in Z/n. Suppose that x ∈ [a] and y ∈
[b]. Then x + y ∈ [a + b] and xy ∈ [ab]. (The brackets means integer but they keep their sign, Z/n means that the number has to be a multiple of n as defined with division a = kb). 

This proposition basically proposes that **modular arithmetic** is true, meaning that [a] + [b] = [a + b] and that [a]•[b] = [ab]. The way you use the modulo operator (≡) is like so; x ≡ (remainder) mod (y) --> x % y = (remainder) --> 14 % 12 = 2. Modular arithmetic might look like so; Z/n, [a] + [b] = [a + b] % n = (remainder) OR [a]•[b] = [ab] % n = (remainder). By the way, moduluoing a smaller number results in a negative remainder number, e.g. 5 ≡ -1 mod 6. 