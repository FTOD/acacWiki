---
tags:
- AbstractInterpretation
- ProgramAnalysis
- ToThink
- DecisionDiagram
---
Within program analyses, the property that the analyses wish to find out is usually represented by some set of states e.g. set of possible values of a variable at a moment, set of cache state at a moment etc.

## Question
A state can often be represented by a tuplet of sub-states:
$S= S_1 \times S_2 \times ...$
The set of states (C stands for *collecting semantics* is then)
$C=\wp(S)$
The question is that, does the set of states can be represented by a state of sets?
let $C^\#=\wp(S_1) \times \wp(S_2) \times ...$ , is $C^\#$ equivalent to $C$?

## Thinking
$C^\#$ is an abstraction of C. 
For example, the concretization of $\gamma( \{x_1, x_2\}, \{y_1, y_2\} ) = \{(x_1, y_1), (x_1, y_2), (x_2, y_1), (x_2, y_2)\}$ 

## Links
#### With XDD?
If we replace the power set by the map of the premise to the corresponding state, what happends?
$S = S_1 \times S_2 \times ...$
$C = \Gamma \rightarrow S$

$C^\# = S_1^\# \times S_2^\# \times ...$ where $S_i^\# = \Gamma \rightarrow S_i$

That means, for a given $\gamma \in \Gamma$, $C[\gamma] = C^\#[\gamma] = \Pi{S^\#_i[\gamma]}$.
I.e. $C$ and $C^\#$ are logically equivalent.


## To Think
In case of using XDD, what are their size? Same?



