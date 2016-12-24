# Tcaingwaq and logic

This is a document showing the logical sentences behind the examples used in the main document.

# 4.

## 4.1.
There are two predicates shown:

* `taq` - talk - a predicate of arity 3;
* `palkei` - potato - a predicate of arity 2.

## 4.2.
Two predicates are merged, expressing a value common to the first argument of both.

* `taq palkei`  
  ∃x\[taq(x) ∨ palkei(x)\]

Swapping the predicates doesn't change the meaning, since the logical disjunction operator (∨) is symmetrical.

* `palkei taq`  
  ∃x\[palkei(x) ∨ taq(x)\] ⇔ ∃x\[taq(x) ∨ palkei(x)\]

## 4.3.
`wa` and `fe` are no different than other predicates. They both are of arity 1.

* `wa taq`  
  ∃x\[wa(x) ∨ taq(x)\]
* `fe palkei`  
  ∃x\[fe(x) ∨ palkei(x)\]

## 4.4.
Since the predicates group in two, the `fe` of the first example starts a new (uncompleted) claim.

`wo` is not an ordinary predicate - it has a referential nature. Because of that, its arity is undefined and depends on context. Moreover, the place filled too depends on the context - it's the earliest place that hasn't been explicitly pointed out.

In this example, it may seem as if `wa taq` and `wo fe` are separate claims; but, because of `wo`, the two parts are bound semantically, and thus logically.


* `wa taq wo fe`  
  ∃x∃y\[wa(x) ∨ fe(y) ∨ taq(x, y)\]

* `wa taq wo fe wo palkei`  
  ∃x∃y∃z\[wa(x) ∨ fe(y) ∨ palkei(z) ∨ taq(x, y, z)\]

## 4.5.
`yu` and `ju` are used for accessing the non-first arguments without `wo`.

* `taq-ju palkei-yu`  
  ∃x\[taq(, , x) ∨ palkei(, y)\]

To be more correct, we can fill the undefined places with anonymous existential variables, yielding:

* `taq-ju palkei-yu`  
  ∃a_1∃a_2∃a_3∃x\[taq(a_1, a_2, x) ∨ palkei(a_3, y)\]

Since all of a_1, a_2 and a_3 could refer to 'me', and this would be probable in most contexts, the addition of 'I' in the translation is reasonable.

## 4.6.
`ro` adds a third predicate to be connected with existential relations.

* `heq taq ro palkei`  
  ∃x\[heq(x) ∨ taq(x) ∨ palkei(x)\]

## 4.7.
`co` is a vague predicate of undefined arity. In the case of connections with `co`, one can represent them in two equivalent ways.

* `co palkei`  
  ∃P∃x\[P(x) ∨ palkei(x)\] (quantification over predicates)  
  ∃x\[palkei(x)\] (ignoring `co`)

# 6.

## 6.1.
`so` is an operator on connections, so it can't be represented with normal logical operators.

* `wa diaq wo so fe beq`  
  ∃x∃y\[wa(x) ∨ so\[fe beq\](y) ∨ diaq(x, y)\]

* `so fe palkei heq`  
  ∃x\[so\[fe palkei\](y) ∨ heq(x)\]

`zo` too is an operator, but instead of quoting a sentence, it creates a new 'compound' predicate.

* `diaq-yu kioq-zo`  
  ∃x\[diaq(, x) ∨ kioqzo(x)\]  
  ∃a_1∃x\[diaq(a_1, x) ∨ kioqzo(x)\]

# 6.2.
As above, `su` creates a new predicate.

* `hyoiq-yu taq-su wo fe`  
  ∃x∃y\[hyoiq(, x) ∨ fe(y) ∨ taqsu(x, y)\]  
  ∃a_1∃x∃y\[hyoiq(a_1, x) ∨ fe(y) ∨ taqsu(x, y)\]