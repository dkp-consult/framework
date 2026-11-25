# Coverage

What each source category can establish about an assumption.

| Category | Can support | Cannot establish |
| --- | --- | --- |
| analytics | observed behavior, funnels, frequency of use | motivation, unmet needs |
| support | reported pain, its frequency and wording | silent users' experience |
| interviews | motivation, context, workarounds | prevalence across all users |
| surveys | stated prevalence and preference | actual behavior |
| billing | conversion, churn, revenue | why customers stay or leave |
| sales | buyer objections and requests | end-user behavior |
| market | public claims, offers, prices | target-user truth |

| Status | When |
| --- | --- |
| `covered` | a declared source whose access is not `none` can support the assumption |
| `unusable` | a declared source could support it, but its access is `none` or its data is not exploitable |
| `missing` | no declared source can support it |

An assumption needing several kinds of support takes the weakest status among them.
