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