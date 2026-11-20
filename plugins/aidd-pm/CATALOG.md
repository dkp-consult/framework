# aidd-pm catalog

Auto-generated index of skills, agents, references and assets shipped by the `aidd-pm` plugin.

> This file is automatically updated by the `scripts/summarize-markdown.js` script.

## Table of Contents

- [`.claude-plugin`](#claude-plugin)
- [`hooks`](#hooks)
  - [`hooks/lib`](#hookslib)
- [`skills`](#skills)
  - [`skills/01-ticket-info`](#skills01-ticket-info)
  - [`skills/02-user-stories`](#skills02-user-stories)
  - [`skills/03-prd`](#skills03-prd)
  - [`skills/04-spec`](#skills04-spec)
  - [`skills/05-spike`](#skills05-spike)
  - [`skills/06-product-brief`](#skills06-product-brief)
  - [`skills/07-epic`](#skills07-epic)
  - [`skills/08-three-amigos`](#skills08-three-amigos)
  - [`skills/09-defect`](#skills09-defect)
  - [`skills/10-task`](#skills10-task)
  - [`skills/11-research-plan`](#skills11-research-plan)
  - [`skills/12-insights`](#skills12-insights)
  - [`skills/13-market-watch`](#skills13-market-watch)
  - [`skills/14-prioritize`](#skills14-prioritize)
  - [`skills/15-impact`](#skills15-impact)

---

### `.claude-plugin`

| File |
|------|
| [plugin.json](.claude-plugin/plugin.json) |

### `hooks`

| File |
|------|
| [artifacts.cjs](hooks/artifacts.cjs) |
| [hooks.json](hooks/hooks.json) |
| [spec-lock.cjs](hooks/spec-lock.cjs) |

#### `hooks/lib`

| File |
|------|
| [host.cjs](hooks/lib/host.cjs) |

### `skills`

#### `skills/01-ticket-info`

| Group | File | Description |
|-------|------|---|
| `actions` | [01-ticket-info.md](skills/01-ticket-info/actions/01-ticket-info.md) | - |
| `assets` | [ticket-template.md](skills/01-ticket-info/assets/ticket-template.md) | - |
| `references` | [tool-detection.md](skills/01-ticket-info/references/tool-detection.md) | - |
| `-` | [SKILL.md](skills/01-ticket-info/SKILL.md) | `Retrieves and shows a ticket from the configured tool when the user wants to see one, not for creating, commenting on, transitioning, or reassigning.` |

#### `skills/02-user-stories`

| Group | File | Description |
|-------|------|---|
| `actions` | [01-frame.md](skills/02-user-stories/actions/01-frame.md) | - |
| `actions` | [02-slice.md](skills/02-user-stories/actions/02-slice.md) | - |
| `actions` | [03-write.md](skills/02-user-stories/actions/03-write.md) | - |
| `actions` | [04-assess.md](skills/02-user-stories/actions/04-assess.md) | - |
| `actions` | [05-estimation.md](skills/02-user-stories/actions/05-estimation.md) | - |
| `actions` | [06-order.md](skills/02-user-stories/actions/06-order.md) | - |
| `actions` | [07-finalize.md](skills/02-user-stories/actions/07-finalize.md) | - |
| `assets` | [user-story-template.md](skills/02-user-stories/assets/user-story-template.md) | - |
| `references` | [estimation.md](skills/02-user-stories/references/estimation.md) | - |
| `references` | [handoffs.md](skills/02-user-stories/references/handoffs.md) | - |
| `references` | [lifecycle.md](skills/02-user-stories/references/lifecycle.md) | - |
| `references` | [ordering.md](skills/02-user-stories/references/ordering.md) | - |
| `references` | [persistence.md](skills/02-user-stories/references/persistence.md) | - |
| `references` | [qualification.md](skills/02-user-stories/references/qualification.md) | - |
| `references` | [readiness.md](skills/02-user-stories/references/readiness.md) | - |
| `references` | [relations.md](skills/02-user-stories/references/relations.md) | - |
| `references` | [slicing.md](skills/02-user-stories/references/slicing.md) | - |
| `scripts` | [contract.json](skills/02-user-stories/scripts/contract.json) | - |
| `scripts` | [validate-story.cjs](skills/02-user-stories/scripts/validate-story.cjs) | - |
| `-` | [SKILL.md](skills/02-user-stories/SKILL.md) | `Produces or refines ordered User Stories from a source when the user wants to slice, write, assess, order, or persist them, not for Epics or code.` |

#### `skills/03-prd`

| Group | File | Description |
|-------|------|---|
| `actions` | [01-draft.md](skills/03-prd/actions/01-draft.md) | - |
| `actions` | [02-finalize.md](skills/03-prd/actions/02-finalize.md) | - |
| `assets` | [prd-template.md](skills/03-prd/assets/prd-template.md) | - |
| `-` | [SKILL.md](skills/03-prd/SKILL.md) | `Generates a PRD from a need, idea, or brainstorm, confirmed before save, when the user wants to draft one, not for user stories or a technical plan.` |

#### `skills/04-spec`

| Group | File | Description |
|-------|------|---|
| `actions` | [01-build.md](skills/04-spec/actions/01-build.md) | - |
| `actions` | [02-refine.md](skills/04-spec/actions/02-refine.md) | - |
| `assets` | [refine-answer.md](skills/04-spec/assets/refine-answer.md) | - |
| `assets` | [spec-template.md](skills/04-spec/assets/spec-template.md) | - |
| `references` | [spec-content.md](skills/04-spec/references/spec-content.md) | - |
| `scripts` | [contract.json](skills/04-spec/scripts/contract.json) | - |
| `scripts` | [validate-spec.cjs](skills/04-spec/scripts/validate-spec.cjs) | - |
| `-` | [SKILL.md](skills/04-spec/SKILL.md) | `Creates or updates a feature's spec, the contract it is built to, when the user brings a need or changes to an existing spec.` |

#### `skills/05-spike`

| Group | File | Description |
|-------|------|---|
| `actions` | [01-create.md](skills/05-spike/actions/01-create.md) | - |
| `actions` | [02-investigate.md](skills/05-spike/actions/02-investigate.md) | - |
| `actions` | [03-conclude.md](skills/05-spike/actions/03-conclude.md) | - |
| `assets` | [spike-template.md](skills/05-spike/assets/spike-template.md) | - |
| `references` | [capabilities.md](skills/05-spike/references/capabilities.md) | - |
| `references` | [investigation.md](skills/05-spike/references/investigation.md) | - |
| `references` | [lifecycle.md](skills/05-spike/references/lifecycle.md) | - |
| `references` | [persistence.md](skills/05-spike/references/persistence.md) | - |
| `references` | [qualification.md](skills/05-spike/references/qualification.md) | - |
| `references` | [relations.md](skills/05-spike/references/relations.md) | - |
| `-` | [SKILL.md](skills/05-spike/SKILL.md) | `Frames, investigates, resumes, or concludes a spike when an uncertainty blocks estimation, feasibility, or design, not for general research or code.` |

#### `skills/06-product-brief`

| Group | File | Description |
|-------|------|---|
| `actions` | [01-frame.md](skills/06-product-brief/actions/01-frame.md) | - |
| `actions` | [02-discover.md](skills/06-product-brief/actions/02-discover.md) | - |
| `actions` | [03-visualize.md](skills/06-product-brief/actions/03-visualize.md) | - |
| `actions` | [04-shape.md](skills/06-product-brief/actions/04-shape.md) | - |
| `actions` | [05-finalize.md](skills/06-product-brief/actions/05-finalize.md) | - |
| `assets` | [product-brief.md](skills/06-product-brief/assets/product-brief.md) | - |
| `references` | [brief-quality.md](skills/06-product-brief/references/brief-quality.md) | - |
| `references` | [evidence.md](skills/06-product-brief/references/evidence.md) | - |
| `references` | [handoffs.md](skills/06-product-brief/references/handoffs.md) | - |
| `references` | [persistence.md](skills/06-product-brief/references/persistence.md) | - |
| `references` | [techniques.md](skills/06-product-brief/references/techniques.md) | - |
| `references` | [visuals.md](skills/06-product-brief/references/visuals.md) | - |
| `-` | [SKILL.md](skills/06-product-brief/SKILL.md) | `Produces a concise Product Brief before requirements. Use when the user wants to frame or revisit a product opportunity and how it will be validated. Not for requirements, technical design, or planning.` |

#### `skills/07-epic`

| Group | File | Description |
|-------|------|---|
| `actions` | [01-shape.md](skills/07-epic/actions/01-shape.md) | - |
| `actions` | [02-review.md](skills/07-epic/actions/02-review.md) | - |
| `actions` | [03-finalize.md](skills/07-epic/actions/03-finalize.md) | - |
| `assets` | [epic-template.md](skills/07-epic/assets/epic-template.md) | - |
| `references` | [handoffs.md](skills/07-epic/references/handoffs.md) | - |
| `references` | [lifecycle.md](skills/07-epic/references/lifecycle.md) | - |
| `references` | [persistence.md](skills/07-epic/references/persistence.md) | - |
| `references` | [qualification.md](skills/07-epic/references/qualification.md) | - |
| `references` | [readiness.md](skills/07-epic/references/readiness.md) | - |
| `references` | [relations.md](skills/07-epic/references/relations.md) | - |
| `-` | [SKILL.md](skills/07-epic/SKILL.md) | `Produces or refines an outcome-based Epic for a product backlog. Use when the user wants to frame, review, resume, or persist an Epic. Not for Product Briefs, User Stories, or implementation.` |

#### `skills/08-three-amigos`

| Group | File | Description |
|-------|------|---|
| `actions` | [01-assess.md](skills/08-three-amigos/actions/01-assess.md) | - |
| `actions` | [02-reconcile.md](skills/08-three-amigos/actions/02-reconcile.md) | - |
| `references` | [assessment.md](skills/08-three-amigos/references/assessment.md) | - |
| `references` | [reconciliation.md](skills/08-three-amigos/references/reconciliation.md) | - |
| `-` | [SKILL.md](skills/08-three-amigos/SKILL.md) | `Assesses an Epic or Story through one product, delivery, or quality lens, then reconciles three caller-supplied reports. Use when the user wants to refine one before a backlog change. Not for spawning or writing.` |

#### `skills/09-defect`

| Group | File | Description |
|-------|------|---|
| `actions` | [01-capture.md](skills/09-defect/actions/01-capture.md) | - |
| `actions` | [02-assess.md](skills/09-defect/actions/02-assess.md) | - |
| `actions` | [03-finalize.md](skills/09-defect/actions/03-finalize.md) | - |
| `assets` | [defect-template.md](skills/09-defect/assets/defect-template.md) | - |
| `references` | [handoffs.md](skills/09-defect/references/handoffs.md) | - |
| `references` | [lifecycle.md](skills/09-defect/references/lifecycle.md) | - |
| `references` | [persistence.md](skills/09-defect/references/persistence.md) | - |
| `references` | [qualification.md](skills/09-defect/references/qualification.md) | - |
| `references` | [readiness.md](skills/09-defect/references/readiness.md) | - |
| `references` | [relations.md](skills/09-defect/references/relations.md) | - |
| `-` | [SKILL.md](skills/09-defect/SKILL.md) | `Produces or refines a backlog Defect from an observed product mismatch. Use when the user wants to report, assess, link, order, transition, or verify a defect. Not for incident response, debugging, or implementation.` |

#### `skills/10-task`

| Group | File | Description |
|-------|------|---|
| `actions` | [01-frame.md](skills/10-task/actions/01-frame.md) | - |
| `actions` | [02-review.md](skills/10-task/actions/02-review.md) | - |
| `actions` | [03-finalize.md](skills/10-task/actions/03-finalize.md) | - |
| `assets` | [task-template.md](skills/10-task/assets/task-template.md) | - |
| `references` | [handoffs.md](skills/10-task/references/handoffs.md) | - |
| `references` | [lifecycle.md](skills/10-task/references/lifecycle.md) | - |
| `references` | [persistence.md](skills/10-task/references/persistence.md) | - |
| `references` | [qualification.md](skills/10-task/references/qualification.md) | - |
| `references` | [readiness.md](skills/10-task/references/readiness.md) | - |
| `references` | [relations.md](skills/10-task/references/relations.md) | - |
| `-` | [SKILL.md](skills/10-task/SKILL.md) | `Produces or refines a backlog Task for bounded delivery work without independent user value. Use when the user wants to create, link, order, estimate, transition, or complete one. Not for User Stories, Spikes, Defects, or implementation.` |

#### `skills/11-research-plan`

| Group | File | Description |
|-------|------|---|
| `actions` | [01-inventory.md](skills/11-research-plan/actions/01-inventory.md) | - |
| `actions` | [02-qualify.md](skills/11-research-plan/actions/02-qualify.md) | - |
| `actions` | [03-method.md](skills/11-research-plan/actions/03-method.md) | - |
| `actions` | [04-kit.md](skills/11-research-plan/actions/04-kit.md) | - |
| `actions` | [05-persist.md](skills/11-research-plan/actions/05-persist.md) | - |
| `assets` | [export-request.md](skills/11-research-plan/assets/export-request.md) | - |
| `assets` | [interview-guide.md](skills/11-research-plan/assets/interview-guide.md) | - |
| `assets` | [po-practices.md](skills/11-research-plan/assets/po-practices.md) | - |
| `assets` | [research-plan.md](skills/11-research-plan/assets/research-plan.md) | - |
| `assets` | [sources.md](skills/11-research-plan/assets/sources.md) | - |
| `assets` | [survey.md](skills/11-research-plan/assets/survey.md) | - |
| `assets` | [watchlist.md](skills/11-research-plan/assets/watchlist.md) | - |
| `references` | [coverage.md](skills/11-research-plan/references/coverage.md) | - |
| `references` | [handoffs.md](skills/11-research-plan/references/handoffs.md) | - |
| `references` | [lifecycle.md](skills/11-research-plan/references/lifecycle.md) | - |
| `references` | [methods.md](skills/11-research-plan/references/methods.md) | - |
| `references` | [persistence.md](skills/11-research-plan/references/persistence.md) | - |
| `references` | [practices.md](skills/11-research-plan/references/practices.md) | - |
| `references` | [qualification.md](skills/11-research-plan/references/qualification.md) | - |
| `references` | [sources-registry.md](skills/11-research-plan/references/sources-registry.md) | - |
| `-` | [SKILL.md](skills/11-research-plan/SKILL.md) | `Produces a research plan turning unproven assumptions into collectable evidence when the user prepares research, not for collecting or synthesizing.` |

#### `skills/12-insights`

| Group | File | Description |
|-------|------|---|
| `actions` | [01-scope.md](skills/12-insights/actions/01-scope.md) | - |
| `actions` | [02-gather.md](skills/12-insights/actions/02-gather.md) | - |
| `actions` | [03-cluster.md](skills/12-insights/actions/03-cluster.md) | - |
| `actions` | [04-confront.md](skills/12-insights/actions/04-confront.md) | - |
| `actions` | [05-persist.md](skills/12-insights/actions/05-persist.md) | - |
| `assets` | [insights.md](skills/12-insights/assets/insights.md) | - |
| `assets` | [po-practices.md](skills/12-insights/assets/po-practices.md) | - |
| `references` | [confrontation.md](skills/12-insights/references/confrontation.md) | - |
| `references` | [handoffs.md](skills/12-insights/references/handoffs.md) | - |
| `references` | [persistence.md](skills/12-insights/references/persistence.md) | - |
| `references` | [practices.md](skills/12-insights/references/practices.md) | - |
| `references` | [rating.md](skills/12-insights/references/rating.md) | - |
| `references` | [scope.md](skills/12-insights/references/scope.md) | - |
| `references` | [signals.md](skills/12-insights/references/signals.md) | - |
| `references` | [sources-registry.md](skills/12-insights/references/sources-registry.md) | - |
| `-` | [SKILL.md](skills/12-insights/SKILL.md) | `Turns customer signals into evidence-rated insights when the user wants to synthesize tickets, interviews, surveys, or exports, not for market watch.` |

#### `skills/13-market-watch`

| Group | File | Description |
|-------|------|---|
| `actions` | [01-scope.md](skills/13-market-watch/actions/01-scope.md) | - |
| `actions` | [02-scan.md](skills/13-market-watch/actions/02-scan.md) | - |
| `actions` | [03-compare.md](skills/13-market-watch/actions/03-compare.md) | - |
| `actions` | [04-persist.md](skills/13-market-watch/actions/04-persist.md) | - |
| `assets` | [insights.md](skills/13-market-watch/assets/insights.md) | - |
| `assets` | [journal.md](skills/13-market-watch/assets/journal.md) | - |
| `assets` | [po-practices.md](skills/13-market-watch/assets/po-practices.md) | - |
| `references` | [comparison.md](skills/13-market-watch/references/comparison.md) | - |
| `references` | [handoffs.md](skills/13-market-watch/references/handoffs.md) | - |
| `references` | [insights-registry.md](skills/13-market-watch/references/insights-registry.md) | - |
| `references` | [persistence.md](skills/13-market-watch/references/persistence.md) | - |
| `references` | [practices.md](skills/13-market-watch/references/practices.md) | - |
| `references` | [scanning.md](skills/13-market-watch/references/scanning.md) | - |
| `references` | [watchlist.md](skills/13-market-watch/references/watchlist.md) | - |
| `-` | [SKILL.md](skills/13-market-watch/SKILL.md) | `Tracks declared competitors with dated, cited observations when the user wants to run or resume a market watch, not for user feedback or one claim.` |

#### `skills/14-prioritize`

| Group | File | Description |
|-------|------|---|
| `actions` | [01-method.md](skills/14-prioritize/actions/01-method.md) | - |
| `actions` | [02-gather.md](skills/14-prioritize/actions/02-gather.md) | - |
| `actions` | [03-score.md](skills/14-prioritize/actions/03-score.md) | - |
| `actions` | [04-rank.md](skills/14-prioritize/actions/04-rank.md) | - |
| `actions` | [05-propose.md](skills/14-prioritize/actions/05-propose.md) | - |
| `assets` | [po-practices.md](skills/14-prioritize/assets/po-practices.md) | - |
| `assets` | [priorities-snapshot.md](skills/14-prioritize/assets/priorities-snapshot.md) | - |
| `references` | [change-set.md](skills/14-prioritize/references/change-set.md) | - |
| `references` | [custom-method.md](skills/14-prioritize/references/custom-method.md) | - |
| `references` | [delta-run.md](skills/14-prioritize/references/delta-run.md) | - |
| `references` | [evidence.md](skills/14-prioritize/references/evidence.md) | - |
| `references` | [handoffs.md](skills/14-prioritize/references/handoffs.md) | - |
| `references` | [methods.md](skills/14-prioritize/references/methods.md) | - |
| `references` | [persistence.md](skills/14-prioritize/references/persistence.md) | - |
| `references` | [practices.md](skills/14-prioritize/references/practices.md) | - |
| `references` | [ranking.md](skills/14-prioritize/references/ranking.md) | - |
| `references` | [scoring.md](skills/14-prioritize/references/scoring.md) | - |
| `references` | [sensitivity.md](skills/14-prioritize/references/sensitivity.md) | - |
| `-` | [SKILL.md](skills/14-prioritize/SKILL.md) | `Ranks one backlog by the recorded method when the user wants to choose a method, score items, or see what flips the order, not for sibling Stories.` |

#### `skills/15-impact`

| Group | File | Description |
|-------|------|---|
| `actions` | [01-arm.md](skills/15-impact/actions/01-arm.md) | - |
| `actions` | [02-measure.md](skills/15-impact/actions/02-measure.md) | - |
| `actions` | [03-judge.md](skills/15-impact/actions/03-judge.md) | - |
| `actions` | [04-persist.md](skills/15-impact/actions/04-persist.md) | - |
| `assets` | [impact-report.md](skills/15-impact/assets/impact-report.md) | - |
| `assets` | [insights.md](skills/15-impact/assets/insights.md) | - |
| `assets` | [po-practices.md](skills/15-impact/assets/po-practices.md) | - |
| `references` | [arming.md](skills/15-impact/references/arming.md) | - |
| `references` | [confounders.md](skills/15-impact/references/confounders.md) | - |
| `references` | [handoffs.md](skills/15-impact/references/handoffs.md) | - |
| `references` | [insights-registry.md](skills/15-impact/references/insights-registry.md) | - |
| `references` | [judgment.md](skills/15-impact/references/judgment.md) | - |
| `references` | [lifecycle.md](skills/15-impact/references/lifecycle.md) | - |
| `references` | [persistence.md](skills/15-impact/references/persistence.md) | - |
| `references` | [practices.md](skills/15-impact/references/practices.md) | - |
| `references` | [sources-registry.md](skills/15-impact/references/sources-registry.md) | - |
| `-` | [SKILL.md](skills/15-impact/SKILL.md) | `Measures whether a released change moved its success signal against a frozen rule when preparing or judging it, not for acceptance or cost checks.` |

