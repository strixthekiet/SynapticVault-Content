---
tags:
  - Math/discrete/Automata
aliases:
  - Finite Automata
  - FA
  - Finite-state Automata
---
# Finite State Machine
### Description:
- Mathematical model of computation  
- Can be in exactly one of a finite number of states at any given time.
- A finite-state automata $M=(S,I,f, s_0, F)$:
	- consists of 
		- a finite set $S$ of states, [[State Space]]
		- a finite input alphabet, $I$
		- a transition funciton $f$, [[Sucessor Function|Transition Function]]
		- an intial or final state, $s_0$
		- a set of possible accepting state, $F$
			- also a subset of $S$
### Types of FA
- FA without output:
	- [[Deterministic Finite-state Automata]]
	- [[Nondeterministic Finite-state Automata]]
- FA with output:
	- [[Moore Machine]]
	- [[Mealy Machine]]
### Transition:
- To change FA from one state to another in response to some inputs
### Accept/reject string:
- A string is said to be **recognized** or **accepted** by the machine, $M=(S,I,f, s_0, F)$, if it takes the initial state $s_0$ to a final state, that is $f(s_0,x)$, is a state in $F$. 
- The **language** recognized or accepted by the machine $M$, denoted by $\color{tomato}L(M)$, is the set of all strings that are accepted by $M$
### Equivalent finite-state automata:
- Definition: Two finite-state automata are called equivalent if they recognize the same language
	- Meaning accept the same set of inputs
### State table:
- ![](https://media.geeksforgeeks.org/wp-content/uploads/20210828221222/capture2.png)