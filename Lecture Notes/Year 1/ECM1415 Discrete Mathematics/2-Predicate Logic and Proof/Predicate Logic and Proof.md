[[ECM1415 Discrete Mathematics for Computer Science]]

3-Oct-2022

### Predicates and Quantifiers

![[Pasted image 20221013233129.png]]

#### Quantifiers

Universal quantifier : $\forall$x. $P(x)$ is true for every x in the domain 

Existential Quantifier : $\exists$x. $P(x)$ is true from some x in the domain

The domain is often denoted by U for universe of discourse

##### Nested Quantifiers

$\forall$x $\exists$y. $(x + y = 0)$

##### De Morgan's Laws for Quantifiers

¬( $\forall$x. $P(x)$ ) $\equiv$ $\exists$x. ¬$P(x)$

¬( $\exists$x. $P(x)$ ) $\equiv$ $\forall$x. ¬$P(x)$


### Rules of Inference

Argument : a sequence of propositions
Premises : all but the final proposition
Conclusion : the last statement
the argument is valid if the premises imply the conclusion

#### Modus Ponens
![[Pasted image 20221013234640.png]]

#### Modus Tollens
![[Pasted image 20221013234702.png]]

#### Other rules
![[Pasted image 20221013234828.png]]

#### Universal Quantifier
![[Pasted image 20221013235005.png]]

#### Existential Quantifier
![[Pasted image 20221013235031.png]]

### Introduction to Proofs

Proof : a valid argument that establishes the truth of a statement
Theorem : a statement that can be shown to be true
Lemma : a helping theorem used to prove a conjecture
Corollary : a result which follows directly from a theory
Conjecture : a statement that is being propsed to be true

#### Direct proof

Assume that p is true. Use rules of inference, axoims, and logical equivalences to show that q must also be true

#### Proof by contraposition

Assume ¬q and show ¬p to conclude p$\implies$q

#### Proof by contradiction

to prove p, assume ¬p and derive a contradiction
if we prove ¬p$\implies$F , it follows that the contrapositive T$\implies$p also holds

#### Proof by cases

sort the conjecture into cases and prove each case

#### Proving biconditional statements

to prove p$\iff$q :
show that p$\implies$q and q$\implies$p are both true

### Mathematical induction

![[Pasted image 20221014152853.png]]

