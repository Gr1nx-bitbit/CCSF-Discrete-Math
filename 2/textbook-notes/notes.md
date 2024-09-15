# Textbook Reading 1.2: Propositional Logic
Truth tables are very laborious to write out so we're going to move over to *propositional calculus* (33). 

## 1.2.1: Tautologies and Contradictions

### Inquiry 1.4 (34):
The sentences are related because they both talk about a relationship between the course and exams i.e. the course grade is dependent on the exam grades like y = 2x

### Inquiry 1.5: Simplify
"If you have a ticket, then, as long as you are wearing a shirt, you may enter the
theater, unless you aren’t wearing shoes." -> if you have a ticket AND are wearing a shirt AND are wearing shoes, you may enter
*Explain equivalence:* All three statements can be negated by each other and shoes can be reversed to be its negative self

### Inquiry 1.6: 
Instead of if then's, you can just sat (condition1 && condition2) || (condition3 && condition4)

**Tautologies** are statements that are ALWAYS true i.e. every single case in a truth table is true
If S -> p is true for all cases then you can rewrite is as S => p and similarly for the <-> logical connective which does to <=>
You can also rewrite (C ^ D) => E to C over D (C/D) } E.

Use a truth table to prove (p -> q)/q } q

|p|q|p -> q|(p -> q) ^ q|[(p -> q) ^ q] -> q|
|-|-|:----:|:----------:|:-----------------:|
|T|T|T|T|T|
|T|F|F|F|T|
|F|T|T|T|T|
|F|F|T|F|T|

A statement whose truth table is ALWAYS false is known as a **contradiction**.

### Ex. 1.6: Show p ^ ¬p is a contradiction

|p|¬p|p ^ ¬p|
|-|:-:|:---:|
|T|F|F|
|T|F|F|
|F|T|F|
|F|T|F|

Statements that are neither contradictions or tautologies (every other statement) is a **contigency**. We can also derive
statements from other statements using tautologies and *derivation rules* (37). Types of derivation rules:
- Equivalence rules:
    - a <=> b: a can deduce b and vice versa
- Inference rules:
    - only works in one direction (a => b): can only deduce b from a
    - You can conclude a weaker statement (T's that line up but also other T's) from a stronger statement.

**Proof sequences** can be used to justify an assertion like a => c. You can have any number of statements in between a and c but they all have to be derived using the derivation rules. 

### Ex. 1.7: Write a proof sequence for for the assertioion p/(p -> q)/(q -> r) } r

p ^ (p -> q) ^ (q -> r) => r | *Modus Ponens*

You can also use current/previous proofs in future proofs

### Ex. 1.8: Prove (p v q)/¬p => q

I don't know what they mean by prove. I'll ask either by email or through office hours. Ok, really it's can you show
through substitutions and transformations that two statements are equal to each other. p -> q == ¬p v q and then make more
and more subs until you find what you're looking for. 

# Textbook Reading 1.3: Predicate Logic

A **predicate** is a declarative sentence whose T/F value depends on one or more unkown variabes. Only after the variables 
have been given values, does the statement become a statement. Predicates also have **domains** or a list/type of value that 
their variables can take (numbers, physical objects, etc.) and is usually stated. Preicates also have **quantifiers** which
quantify the validity of variables. For example, the universal quantifier (**V**x)E(x) says that EVERY value for that variable
will give a true result, while the exstistential quantifier (**∃**x)E(x) says that SOME values of x gives a true result for E(x).
Really, the power of predicate logic comes in giving propositional logic flexibility. The **scope** of a quantifier is usually the
set of parenthases directly after itself e.g. (Vx)(_...scope of Vx_...), (∃x)(_...scope of ex..._). 

Negation is pretty straightfoward. ¬[(Vx)E(x)] --> (∃x)[¬E(x)]. This leads up to manipulating propositional logic like before but with
free variables. 