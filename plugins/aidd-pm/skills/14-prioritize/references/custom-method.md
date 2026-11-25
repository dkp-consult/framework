# Custom method

Build a method with the user, one question at a time, in this order.

| Step | Ask | Accepted answer |
| --- | --- | --- |
| goal | what the ranking must favor | one sentence, for example retention over acquisition |
| criteria | which factors decide it | two to five names, effort or size included |
| direction | whether each criterion raises or lowers the score | raises or lowers |
| scale | how each criterion is measured | a count, a bounded number range, or named levels mapped to numbers |
| weight | how much each criterion counts | a number per criterion, or equal weights |
| formula | how criteria combine | a weighted sum, a ratio, or a product; lowering criteria divide or subtract |
| evidence | which artifact or source sets each criterion | a kind named in `evidence.md`, or a declared source category |
| mapping | which evidence condition gives each point of the scale | one condition per point, or a conversion from the estimation scale for effort |
| thresholds | where high splits from low, when the formula reads quadrants | one point per criterion |

| Check | Result |
| --- | --- |
| criterion without a scale | not usable; ask for one |
| criterion without an evidence kind | not usable; ask for one |
| criterion without a mapping | not usable; ask for one |
| quadrants without thresholds | not usable; ask for them |
| two criteria measuring the same thing | ask whether to merge them |
| no effort or size criterion | ask whether cost is deliberately ignored |
| formula naming an undefined criterion | not usable; ask for the missing definition |

A usual method the user adapts follows the same checks for each changed criterion.
