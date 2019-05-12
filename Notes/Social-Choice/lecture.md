# Social Change

## Preferences
* Given a finit set of outcomes or alternatives $O$.
* Agent have (strict) preferences, $\succ$, over the outcomes: linear orders (or total orders)
* Linear orders L: binary relations $\succ$ that are total and transitive
	* total: for ever pair of outcomes $a\not=b$ either $a\succ b$ or $b \succ a$ (but not both: so it is complete and antisymmetric)
	* transitive: $a \succ b$ and $b \succ c$ implies $a \succ c$
* Non-stric preferences $L_{NS}$: binary relations $\succeq$ that are complete and transitive
	* complete: for every $a,b$ either $a \succeq b$ or $b \succeq a$ (both indicates indifference)
	* transitive: $a \succeq b$ and $b \succeq c$ implies $a \succeq c$

## Formal Model
Given a set of agents $N = \{1,2,\dots,n\}$ a finite set of outcomes (or alternatives, or candidates) $O$, and the linear orders on the outcomes, $L_{NS}$.

**Definitions**
- A *social choice function* is a function $C: L^{n}_{NS} \rightarrow O$
- A *social welfare function* (or social welfare ordering) is a function $W: L^{n}_{NS} \rightarrow L_{NS}$


## Voting Schemes: Scoring Rules

* Plurality
	* pick the outcome which is most-preferred by the most people
* Comulative Voting
	* distributive e.g., 5 votes each
	* possbile to vote for the same outcome miltiple times
* Approval voting
	* vote for as many outcomes as you like
* Plurality with elimination ("instant runof", "transferable voting")
	* if some outcomes has a majority, it is the winner
	* otherwise, the outcome with the fewest votes is eliminated (may need some tie-breaking procedure)
	* repeat until there is a winner
* Borda Rule, Borda Count
	* assign each outcome a number
	* The most preferred outcome get a score of $n-1$, the next most preferred gets $n-2$, dow to the $n^{th}$ outcomes which gets 0.
	* Sum scores for each outcome and choose one with highest score.
* Successive elmination
	* in advance, decide an ordering of alternatives
	* everyone votes for the first or second and the loser is eliminated

## Condorcet Consistency

If there is a candidate or outcome that is preffered to every other candidate in pariwise majority-rule comparisons, that candidate should be chosen.
* There is not always a Condorcet winner
* sometimes, there is a cycle where A defeats B, B defeats C, and C defeats A, known as a Condorcet Cycle
