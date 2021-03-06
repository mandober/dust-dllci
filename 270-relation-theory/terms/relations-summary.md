# Sets: Summary



- inclusion relation is reflexive, transitive, and anti-symmetric
- proper inclusion relation is irreflexive, transitive, and asymmetric. 
- inclusion and proper inclusion relations have natural converses;
  A (properly) includes B iff B is (properly) included in A;
  alternatively, A is a (proper) superset of B
- exclusion relation is symmetric and anti-reflexive

- subset is an example of inclusion relation
- inclusion relation is antisymmetric
- set membership (belonging) is an example of membership relation
- membership (elementhood) relation is reflexive
- inclusion relation is transitive, membership relation is not

## Relations: Summary


(x,y) ∈ R 
or 
xRy (x is "R-related" to y)

R: X -> Y

A relation $$R$$ from set $$X$$ (domain) to set $$Y$$ (codomain), where $$x \in X$$ and $$y \in Y$$, is denoted as $$(x,y) \in R$$ or $$xRy$$ (x is R-related to y).

If the sets are equal, the Cartesian product, $$X\times X$$, is denoted by $$X^2$$ and a relation is $$xRx$$

**A relation is a subset** of the Cartesian product, $$R \subseteq X\times Y$$

**A relation is an element** of the powerset of the Cartesian product of sets, $$R \in \mathcal{P}(X\times Y)$$

Total number of relations of an n-element set with itself is $$|\mathcal{P}(X^2)| = 2^{n^2}$$


## Sets
- Cardinality of the set X is denoted by $$|X| = n$$
- Cardinality of the powerset of the set X is $$|\mathcal{P}(X)| = 2^{|X|} = 2^n$$
- Cardinality of the Cartasian product of the set X: $$|X \times X| = |X^2| = n^2$$
- Cardinality of the powerset of the Cartasian product of the set X is $$|\mathcal{P}(X^2)| = 2^{(n^2)}$$
- Each relation is a subset of the Cartasian product of the set X: $$R \subseteq X^2$$
- Each relation is an element in the powerset of the Cartasian product of the set X: $$R \in P(X^2)$$
- Number of all possible relations on a $$X^2$$ set: $$|\mathcal{P}(X^2)| = 2^{(n^2)}$$

- standard set notation: curly braces for listing the elements explicitly
- comprehensions: `{x ∈ S |...}`
- `∅` for the empty set
- `S \ T` for the set difference of `S` and `T`
- cardinality of a set `S` is `|S|`
- powerset of `S` i.e. the set of all the subsets of `S`, is `P(S)`
- the set `{0,1,2,3,4,5,...}` of natural numbers is denoted by the symbol `N`
- a set is countable if its elements can be placed in one-to-one correspondence with the natural numbers


## Relations
- An n-place relation on a collection of sets `S1,S2,...,Sn`
  is a set `R ⊆ S1 × S2 ×...× Sn` of tuples of elements `S1 - Sn`
- the elements `s1 ∈ S1` through `sn ∈ Sn` are related by `R` if `(s1,...,sn)` is an element of `R`
- A one-place relation on a set `S` is called a predicate on `S`
- P is true of an element `s ∈ S` if `s ∈ P`
- we write `P(s)` instead of `s ∈ P`, regarding `P` as a function mapping elements of `S` to truth values
- A two-place relation `R` on sets `S` and `T` is a binary relation
- We write `sRt` instead of `(s, t) ∈ R`
- if `S` and `T` are the same set `U`, then `R` is a binary relation on `U`
- 3-place or more place relations are often written using a mixfix concrete syntax, where the elements in the relation are separated by a sequence of symbols that jointly constitute the name of the relation. For example, for the typing relation for the simply typed lambda calculus, we write `Γ ⊢ s : T` to mean the triple `(Γ,s,T)` is in the typing relation.
- The domain of a relation R on sets S and T, written `dom(R)`, is the set of elements `s ∈ S` such that `(s, t) ∈ R` for some `t`.
- The codomain or range of `R`, written `range(R)`, is the set of elements `t ∈ T` such that `(s, t) ∈ R` for some s


## Functions

- A relation R on sets S and T is called a partial function from S to T if, whenever `(s, t1) ∈ R` and `(s, t2) ∈ R`, we have `t1 = t2`.
- If, in addition, `dom(R) = S`, then R is called a total function (or just function) from S to T. 
- A partial function R from S to T is said to be defined on an argument `s ∈ S` if `s ∈ dom(R)`, and undefined otherwise.
- We write `f (x) ↑`, or `f (x) =↑`, to mean _f is undefined on x_, and `f (x)↓` to mean _f is defined on x_
- we also need to define functions that may fail on some inputs, so it is important to distinguish failure (which is a legitimate, observable result) from divergence
- a function that may fail can be either partial, i.e. it may also diverge, or total (it must always return a result or explicitly fail)
- We write `f(x)=fail` when f returns a failure result on the input x.
- Formally, a function from S to T that may also fail is actually a function
from S to `T ∪ {fail}`, where we assume that `fail` does not belong to T.
- Suppose R is a binary relation on a set S and P is a predicate on S. P is preserved by R if whenever we have `sRs'` and `P(s)`, we also have `P(s0)`.
