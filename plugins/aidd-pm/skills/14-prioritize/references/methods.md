# Methods

Five usual methods. Each mapping below is a proposal made at method choice; the one the user approves is recorded with the method.

| Method | Formula | Fits when |
| --- | --- | --- |
| RICE | reach x impact x confidence / effort | reach can be counted from insights or analytics |
| WSJF | (value + time criticality + risk reduction) / job size | delay has a cost: deadlines, market moves, blocked work |
| ICE | impact x confidence x ease | evidence is thin and a quick relative pass is enough |
| value/effort | value / effort, read as quadrants | the team wants quick wins and big bets apart |
| MoSCoW | category, no formula | a release scope must be cut, not a full order |

## Need levels

Several mappings below read the need level of an item. Insight rows state no level: the product owner gives it per item, as `scoring.md` records it.

| Level | The product owner judges |
| --- | --- |
| critical | the outcome fails without the item |
| blocker | a recurring blocker for a segment |
| friction | a recurring friction for a segment |
| occasional | an occasional friction |
| preference | a preference only |

## RICE

| Criterion | Scale | Evidence it needs | Proposed mapping |
| --- | --- | --- | --- |
| reach | users or accounts per period, a count | insight Frequency and Segment, or an analytics source | the count read, over the period recorded |
| impact | 0.25, 0.5, 1, 2, 3 | insight rows with Effect `supports` or `new`, an impact report on similar work | critical 3, blocker 2, friction 1, occasional 0.5, preference 0.25 |
| confidence | 50%, 80%, 100% | the Confidence of the rows cited for reach and impact | lowest cited row: `low` 50%, `medium` 80%, `high` 100% |
| effort | project scale | the item's estimate | the estimate as written |

## WSJF

| Criterion | Scale | Evidence it needs | Proposed mapping |
| --- | --- | --- | --- |
| value | 1, 2, 3, 5, 8, 13, 20, relative | insight rows on the need, an impact report on similar work | critical 20, blocker 13, friction 5, occasional 2, preference 1 |
| time criticality | 1, 2, 3, 5, 8, 13, 20, relative | a dated obligation, a market row naming a market standard | obligation due within the next release 20, market standard row 8, no date and no market row 1 |
| risk reduction | 1, 2, 3, 5, 8, 13, 20, relative | an open research plan or Spike the item settles, items it unblocks | settles a gap gating other items 13, unblocks one item 5, neither 1 |
| job size | project scale | the item's estimate | the conversion the user records from the estimation scale |

## ICE

| Criterion | Scale | Evidence it needs | Proposed mapping |
| --- | --- | --- | --- |
| impact | 1 to 10 | insight rows on the need, an impact report on similar work | critical 10, blocker 7, friction 5, occasional 3, preference 1 |
| confidence | 1 to 10 | the Confidence of the rows cited for impact | lowest cited row: `low` 2, `medium` 5, `high` 8 |
| ease | 1 to 10, the inverse of effort | the item's estimate | the conversion the user records from the estimation scale; none recorded gives `unknown` |

## Value/effort

| Criterion | Scale | Evidence it needs | Proposed mapping |
| --- | --- | --- | --- |
| value | 1 to 5 | insight rows on the need, market rows, an impact report | critical 5, blocker 4, friction 3, occasional 2, preference 1 |
| effort | project scale | the item's estimate | the estimate as written |

The value and effort points splitting high from low are recorded with the method; none is proposed by default.

| Quadrant | Value | Effort | Order |
| --- | --- | --- | --- |
| quick win | high | low | first |
| big bet | high | high | second |
| filler | low | low | third |
| money pit | low | high | last |

## MoSCoW

| Category | Evidence condition |
| --- | --- |
| must | the outcome fails without it, or a dated obligation applies |
| should | insight rows at `medium` or above, no obligation |
| could | a `low` row or a market row only |
| won't | the user excludes it for this scope |

Items share a category unordered; dependencies and the user order them inside it.
