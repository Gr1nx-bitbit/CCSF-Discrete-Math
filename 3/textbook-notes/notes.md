# Textbook Reading 1.4

**Defnitions** in math texts are not just descriptions of an object or action; they are REQUIREMENTS for a symbol, term, or something else e.g. definition: lines are parallel if they have no intersections

To **prove** something mathematically, you need to use the definitons given to you e.g. an integer n is odd IF AND ONLY IF n = 2k + 1, k an integer -> 17 is odd because 17 = 2*8 + 1. You CANNOT have more than one definiton for a single term. <font color="red">Definitions are logical "if an only if" <--> statements!!</font> Usually definitons are written as [Object] *x* is [defined term i.e. even || an integer] if [definiting property i.e. x = 2k, k an integer || integer defining prop] --> D(x) = x is [defined term], P(x) = [x definig property], (Vx)(D(x) <--> P(x)).

**Axioms** or **postulates** are your basic building terms. We need some statement to build off of otherwise it would be impossible to prove anything. These guys are fundamental and basic assumptions about the/your world. **Theorems** are logical statements that follow existing axioms, definitons, and or other theorems. **Proofs** are statements/arguments that prove the validity/truth of a statement or theorem using definitons, proven theroems, and or axioms. 

Usually math statements are like (Vx)P(x), and we know the negation. Only one or the other can be true but not both, therefore if you find a ¬P(x) then you know (Vx)P(x) is false. A **counterexample** is like the ¬P(x) or something that shows the original statement to be false.

**Axiomatic Systems** have **undefined terms** (these guys are abstractions and have no formal meaning) which act as the starting vocabulary for a system e.g. a system for four point geometry --> undefined terms: point, line, is on, etc. Some undefined terms can be better defined as definitons but you will need some undefined terms to start with. **Models** are a specific context in which all undefined terms have meaning and all the axioms are true.

# Textbook Reading 1.5

*Inquiry 1.13*: Suppose that a and b are odd integers. What can be said about their sum a + b? Explain your reasoning.
An odd integer is defined as i = 2k + 1, k an integer. If we were to add two odd integers together (2k + 1) + (2n + 1), k, n integers then the resulting equation would be 2k + 2n + 2. We can factor out the two giving us 2(k + n + 1) which gives us an even integer, thus, the sum of two odd integers is an even integer

*Inquiry 1.14*: What can be said about the sum of two even integers? Explain.
An even integer is defined as i = 2k. If we were to add two even integers together and factor the two out --> 2(k + n), then we would have an even integer no matter what, therefore, two even integers summed together result in an even integer. 

Direct proofs are a sequence of statements and reasons (*A* => B1 => B2 => ... => Bn => *C*) **where each conclusion is supported by an axiom or other term**. 

Ex 1.19: Prove the following statement: For all real numbers x, if x > 1, then x^2 > 1.
Uhh, ok, so idk what our axioms are definitons are. But basically we're showing that for x > 1, x multiplied by itself is greater than 1 as well. Do we rewrite the equations / make them equal to each other? Start with a contradication or contraposition? --> Ohh, ok, so we can manipulate the given expression to get to the desired one. x > 1, if we multiply by another real number on both sides, the inequality is preserved, x^2 > x, and since x > 1, x^2 > 1. 

**Rule of Thumb 1.1**: To prove a predicate implication for all the domain (Vx)(P(x) --> Q(x)), start your proof with let x be an [element of the domain], and suppose P(x) is true. 

**Definition 1.10**: An integer x *divides* an integer y if there is some integer k such that y = kx. We write x | y if x divides y.

**Axiom 1.1**: If *a* and *b* are integers, so are *a* + *b* and *a* · *b*. 

Ex. 1.20: Prove the following: For all integers a, b, and c, if a | b and a | c, then a | (b + c)

For an integer to divide another integer, then that means b = ka, k an integer and c = na, n an integer. This sentence was correct. 

Let a be an integer and Suppose that a | b and a | c. a | b means that b = ka. a | c means that c = na. Therefore if a | (b + c) then b + c = ka + na. Then b + c = a(k + n). b + c must also equal an integer via axiom 1.1, therefore b + c = d an integer. I don't know where I'm going with this. Wait this is right. Dude, I don't know whent to stop lol. I think I just have to keep the definitions and axioms in my mind. **<font color="green"> OK, so the strat is to use definitions to define things, use axioms to manipulate your equations and then use definitons again to justify your manipulations </font>**

#### Proof By Contraposition
This is a method you can use when you get stuck on trying to prove something. Basically you try to prove the contrapositive of the statement which is it's logical equivalent. 

**Rule of Thumb 1.2**To prove a statement of the form (∀x)(P(x) → Q(x)), begin your proof with a sentence of the form: let x be an [element of the domain] and suppose ¬Q(x). This proof starts with assuming ¬Q(x) is true and following a sequence of statements showing that ¬P(x) is true. 

For Euclidean Geometry we have a theorem
**Theorem 1.2**: The sum of the measures of the angles of any triangle equals 180°

**Definition 1.11**: Two lines are parallel if they do not intersect

This is confusing man, but I think I can get through it if I just know the definitons

#### Proof by Contradiction
With this, to prove a statement, start with its negation and then prove something you know to be false. 

**Rule of thumb 1.3**: To prove a statement A by contradiction, begin your proof with the following sentence: Suppose, to the contrary, that ¬A is true

Ex 1.23 In Euclidean geometry, prove: The statement in English is: If two lines share a common perpendicular, then the lines are parallel.
The predicate logic form is of this: x is a line, y is a line, C(x, y) means x and y have a common perpendicular, P(x, y) means x and y are parallel. (∀x)(∀y)(C(x, y) → P(x, y)). Then the negation of the statement is ¬[(∀x)(∀y)(C(x, y) → P(x, y))] which goes to (∃x)(∃y)¬(¬C(x, y) v P(x, y)) which goes to (∃x)(∃y)(C(x, y) ^ ¬P(x, y)). This last statement means there exists some line x and y that have a common perpendicular and are not parallel. So we're trying to show that two lines have a common perpendicular but are not parallel. The books solution goes like so: if we have two lines that are not parallel, then they intersect. Since they have a common perpendicular though that means they both have right angles with the intersection. So the triangle made by the lines x, y, and the point P need to have two right angles and then an angle of 0° measure. That is false by theorem 1.2.

**Definition 1.5**: An integer n is even if n = 2k for some integer k.
**Definition 1.6**: An integer n is odd if n = 2k + 1 for some integer k.
**Axiom 1.2**: For all integers n, ¬(n is even) ⇔ (n is odd).

Prove the Lemma 1.1 Let n be an integer. If n^2 is even, then n is even.

So to prove by contradiction we negate the statement.
n is an even integer, S(n) means n^2 is even, E(n) means n is even. (∀n)(S(n) -> E(n)) We negate the statement ¬[(∀n)(S(n) -> E(n))] which goes to ¬[(∀n)(¬S(n) v E(n))] which goes to (∃n)(S(n) ^ ¬E(n)) which means that for some integer n, it is even when squared and odd when not. That means n^2 is an even integer = 2k while n itself is odd which means n = 2i + 1. n^2 = (2i + 1)(2i + 1) which has to equal 2k. So 2k = (2k + 1)^2 => 2k = 4k^2 + 4k + 1, 1 the right side of the equation is odd because of 1 and the left side of even. Therefore that is a contradiction by axiom 1.2

Ex 1.24: Prove 2^(1/2) is irrational
A rational number is one where a/b is possible, a and b are integers, and b ≠ 0. Suppose the contrary, that 2^1/2 is rational. That means that there is some integer b that divides into a to produce the number. Therefore a = nb where n is an integer. They went on to talk about lowest terms which i don't even know what that is. 

x is in the domain of algebraic varieties: G(x) means x has a generic point -> (Vx)(G(x)) all algebraic varieties have a generic point, ¬[(Vx)(G(x))] --> (Ex)(¬G(x)) means there exists some algebraic variety that does not have a generic point

AoC -> WOP, contrapositive is ¬WOP -> ¬AoC