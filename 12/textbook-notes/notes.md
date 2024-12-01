# Textbook Reading 4.5: Counting Operations in Algorithms
This is just simple pseudocode - we already know how to do this :)

# Textbook Reading 4.6: Estimation

**Definition 4.6** et f : N → R+ be a function. Then O(f) is the set of all functions g such that *g(n) ≤ Kf(n)* for some constant K > 0, and for all n ≥ N for some N > 0. If g ∈ O(f), we also say that “g is big-oh of f.” --> the key to this definition is the inequality "≤" | this is also the worst case

**Definition 4.7** Let f : N → R+ be a function. Then Ω(f) is the set of all functions g such that *g(n) ≥ Kf(n)* or some constant K > 0, and for all n ≥ N for some N > 0. If g ∈ Ω(f), we also say that “g is big-omega of f.” --> this is the best case

**Definition 4.8** Let f : N → R+ be a function. The big-theta class Θ(f) is the set of all functions g such that *K[1]f(n) ≤ g(n) ≤ K[2]f(n)* for some positive constants K1, K2, and for all n ≥ N for some N > 0. In other words, Θ(f) = O(f) ∩ Ω(f). If g ∈ Θ(f), we also say that “g is big-theta of f” or “g is order f.” --> this guy can be used for comparison between functions

Theorem 4.12 - a list of time complexities from best to worst:
1. 1
2. log2(n)
3. n^p for 0 < p < 1
4. n
5. nlog2(n)
6. n^p 1 < p < infinity
7. 2^n
8. n!

**Theorem 4.13** Let f : N → R+ be a function, and let k > 0 be a constant. Then k f(n) ∈ Θ(f(n)). --> basically, multiplying a function by a constant doesn't really change anything in terms of how it scales up

**Theorem 4.14** Let f, g : N → R+be functions, and suppose that g(n) ∈ O(f (n)). Then f (n) + g(n) ∈ Θ(f (n)). --> idrk what this theorem is saying - the text touches on how the biggest factor is the one that we estimate i.e. 1 + 2^n is just 2^n or n! + 2^n is just n!

