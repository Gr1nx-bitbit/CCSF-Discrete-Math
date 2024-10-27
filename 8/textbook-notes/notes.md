# Reading 3.3: Recursive Definitions
An **object** is a pretty loose term, it just refers to the thing we want to define recursively. We can define an object in recursive terms with its **base case (B)** which describes the simplest object possible and its **recursive case (R)** which defines a more complex object in terms of simpler objects. A recursive definition can also have *MORE than a single base case!!* I don't think this would be true for recursive cases unless you could transition between separate recursive cases reliably - nevermind, you can have multiple recursive cases (example 3.17) - it seems like if you want multiple recursive cases, they have to have the same effect on the object, just coming from different conditions - would some conjugation then be multiple recursive forms?? A **string** is a sequence of symbols, the same thing as in CS. 

**Theorem 3.1** (for strings) If *a* is a symbol (CS character) then a^R = a. 

Ex 3.20 Suppose you start browsing the Internet at some specified page p. Let X be the set of all pages you can reach by following links, starting at p. Give a recursive definition for the set X. --> The base case would be B. p in the set of X, then the recursive case would give you a page that comes from within the set and set your new "base" to that new page instead of p | **S** if x is a page in X and y is some page that links to x then y is also in X. 

Ex 3.21 Give a recursive definition for the set of all odd natural numbers (positive odd integers). --> Our base case would be B. 1, and we know the definiton of an odd number to be 2k + 1, k an integer, therefore our recursive case becomes R. 2(n) + 1. | **S** B. 1 is in X, R. if x is in X then so is x + 2. 

# Reading 3.4: Proof by Induction
*Inquiry 3.9*: A function f : Z → Z is called parity preserving if f(n) is even when n is even and if f(n) is odd when n is odd. Give an example of a parity-preserving function (besides the identity). Explain how you know that the function preserves parity. --> f(x) = x + 2, we can prove this via using odd numbers, 2k + 1, if we add two to this then we get 2k + 3, but 3 itself can be defined as 2n + 1 so the equation goes to 2k + (2n + 1) = 2(k + 1) + 1 which is an odd number.

*Inquiry 3.11* --> We get the result because every time we add a vertex in this manner the number of edges goes up by two while the number of vertecies only goes up by one, the difference therefore is one. 

Remember, to prove a recurrence realtion is the same as its closed form solution, we first have to prove that R(1) = f(1) and that R(n) = f(n). For mathmateical induction we follow the same reasoning as before showing S(1) is true and that S(n - 1), n ≥ 1, is also true which builds up our chain of implications. <font color="green">The template for proving stuff by induction is showing that an object (which can be defined recursively) has a property P for all of its forms is:
    - **Base case**: Prove the simplest object has the porperty P
    - **Inductive Hypothesis**: Suppose the property holds for the object at level k - 1
    - **Inductive Step**: Use inductive hypothesis and recursive definition to conclude that level k of the object has property P </font>
Sometimes recurrence relations use multiple previous steps so you will need a stronger inductive hypothesis, one that covers all of your base cases. **Strong induction** means that your next level relies on ALL previous levels. 

Ok, so you also have to assume things about your proofs or set qualities that you want to keep. For example, they just proved that is x is in the set of X, then x - 12 and x^2 are both divisible by 4 and therefore are in x, **HOWEVER, THEY ASSUMED THAT x ITSELF WAS DIVISIBLE BY 4, SO YOU CAN ASSUME CERTAIN THINGS TO SHOW THAT YOUR PROOF WORKS SO LONG AS THOSE CONDITIONS HOLD**.