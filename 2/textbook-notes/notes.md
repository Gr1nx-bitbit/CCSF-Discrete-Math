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