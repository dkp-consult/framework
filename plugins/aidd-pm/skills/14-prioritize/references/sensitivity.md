# Sensitivity

Sensitivity names the smallest change that would flip a position.

| Case | Statement |
| --- | --- |
| an `unknown` criterion could flip two adjacent items | if the criterion of B is at least the threshold, B passes A |
| a flagged `low` value could flip them | if that row is confirmed or contradicted, the order becomes the one named |
| one effort step could flip them | if A's effort is one step higher, B passes A |
| a user assumption could flip them | if that assumption is wrong, the order becomes the one named |
| overlapping score ranges | order undecided until the named criterion is known |
| no change within the scales flips them | stable |

| Rule | Detail |
| --- | --- |
| scope | every adjacent pair, plus any pair whose ranges overlap |
| threshold | the exact criterion value where the scores meet, on the criterion's scale |
| several flipping changes | the one needing the least new evidence first |
| decisive unknown | an `unknown` that flips a top position is offered for collection |
