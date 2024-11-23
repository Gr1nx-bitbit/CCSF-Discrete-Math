# Textbook Reading 4.3: Counting with Functions

**Theorem 4.4** Let |X| = m and |Y| = n. If there is some f : X → Y that is one-to-one, then m ≤ n. --> i'm a little confused, if a function is one to one, that means every element in the domain has a unique counterelement in the codomain. Wouldn't that m can only be equal to n?

**Theorem 4.5** Let |X| = m and |Y| = n. If there is some f : X → Y that is onto, then m ≥ n. --> This makes sense since if the function is onto and one to one then m = n, and if we have a function like y = x^2 then we have 2n - 1 elements for the x domain and n elements for the y domain. 

**Corollary 4.2** Let |X| = m and |Y| = n. If there is a one-to-one correspondence f : X → Y, then m = n. --> basically if there is a one-to-one correspondence between two finite sets, then they have the same number of elements. 

Basiaclly, the idea behind counting with functions is to find a one to one correspondence (patterm) between elements of the codomain and a subset or the set of elements in the domain. Find a one to one correspondence with Y and X and then count X instead. 

**Definition 4.1** A function f : X → Y is called n-to-one if every y in the image of the function has exactly n different elements of X that map to it. In other words, f is n-to-one if |{x ∈ X | f(x) = y}| = n for all y ∈ f(X). 

**Theorem 4.6** Let |X| = p and |Y| = q. If there is an n-to-one function f : X → Y that maps X onto Y, then p = qn. --> basically, if there are 'n elements' ∈ X for 'every elemtent' ∈ Y, then |X| = n|Y|. 

The PigeonHole Principle (PHP) says that if we have n pigeons and r holes and that n > r then some hole(s) will have multiple pigeons in it --> **Theorem 4.7** Let |X| = n and |C| = r, and let f : X → C. If n > r, then there are distinct elements x, y ∈ X with f(x) = f(y). --> ah, ok, so if there are more elements in X than in Y then more than one element in X will map to the same element in Y. 

A more general version of the PHP is that if there are way more pigeons than holes, there will be a hole with a lot of pigeons in it. --> **Theorem 4.8** Let |X| = n and |C| = r, and let f : X → C. If n > r(l − 1), then there is some
subset U ⊆ X such that |U| = l and f (x) = f (y) for any x, y ∈ U. --> basically if the cardinality of X is greater than the cardinality of C to an extent, then there exits a subset within X whose elements all map to the same codomain value.

# Textbook Reading 4.4: Discrete Probability
Probabilty is what we think the liklihood of something happening on a scale from 0 to 1. Probability, in mathmateical terms, is the ratio of some elements in another set as in, how many elements from set U are in a subset A? 

**Definition 4.2** Suppose A is a subset of a nonempty finite set U. The probability that a randomly chosen element of U lies in A is the ratio P(A) = |A| / |U| - U is called the *sample space* and A is called an *event*. You have to be careful about defining your Sample space!!

**Theorem 4.10** Let A be a subset of a nonempty finite set U. Let A′be the complement of A in U. If P(A) = p, then P(A′) = 1 − p