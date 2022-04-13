---
aliases: [Soundness, Completeness]
tags:
- FormalSystem
- Soundness
- Completeness
---

A logical system is equipped a syntactic entailment $\vdash$ and semantic entailment $\models$.

### Soundness
A system is sound iff. every formula that can be proved in the system i.e. with the logical language defined by the syntax of the system, is logically valid with respect to the semantics of the system. That is, if $\Gamma \vdash C$, then $\Gamma \models C$.

In another word, anything that can be proven true by the system is true (according to the semantics).

### Completeness
The completeness of the system is the converse of its soundness: a system is sound iff. every theorem that is true in the semantic is provable with the syntax i.e. axiomes and inference rules. That is, if  $\Gamma \models C$, then $\Gamma \vdash C$.

In another word, anything that is true can be proven.

#### Connection with the soundness in program analysis
In program analysis, we call an analysis is sound if it does not give any false result. It may assert "don't know", but when it is certain of TRUE or FALSE, the semantic is TRUE or FALSE. That means the analysis is sound but not complete.

