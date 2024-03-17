---
tags:
  - Math/discrete/Automata
aliases:
  - NFA
---
# Nondeterministic Finite-state Automata
### Description:
- Can have multiple state from one state given an input
- The transition function $f$ assigns **a set of states** to each pair of state and input (so that $f:S\times I\to \mathcal P(S)$ )
### NFA's recognized language:
- Let a string $𝑥=𝑥_1 𝑥_2…𝑥_𝑘$ input to an NFA.
- The first input symbol $𝑥_1$ takes the starting state $𝑠_0$ to **a set $𝑆_1$ of states**
- The next input symbol $𝑥_2$ takes **each of the states in $𝑆_1$ to a set of new states**. 
	- Let $𝑆_2$ be the union of these sets.
- Repea, at each stage, all states obtained using a state obtained at the previous stage and the current input symbol
- The string $𝑥$ is accepted if there is **at least 1 final state in the set of all states** using $𝑥$.
- The language recognized by a NFA is the set of all strings recognized by this NFA.
- #Math/discrete/Automata/theorem
	- If the language $L$ is recognized by a NFA, $M_0$, then $L$ is also recognized by a [[Deterministic Finite-state Automata|DFA]] $M_1$
		- where $M_1$ (deterministic) is converted from $M_0$ (Non-deterministic)
		- $M_1$'s states are created from combinations of possible states reached by $M_0$'s states 
			- with **OR** operation
			- combination states where each state can have multiple possible states, the new state of $M_1$ is all of those possible states.
---
