# Handoffs

Offer the named capability with what was observed, then stop. Never invoke it silently, never write outside an Epic.

| Observed | Capability | Return |
| --- | --- | --- |
| one independently deliverable behavior | User Story | one-way; no Epic is created |
| work without independent user value | Task | one-way |
| observed product mismatch | Defect | one-way |
| several outcomes that succeed independently | Epic, one per outcome | replaces this draft |
| uncertainty blocking readiness | Spike | review resumes after its outcome |
| outcome or need resting on an assumption that no evidence checks before building | Research plan | review resumes once the evidence is collected; measuring after delivery instead only when the user explicitly accepts that risk |
| the outcome is settled enough to slice | User Story | the Stories are sliced from it |
| several Epics competing for the same capacity | a prioritization capability | ordering resumes with the decided order |
| Epic becomes `ready` with a success signal | an impact capability | arms the measurement before release; the Epic is unchanged |
| Epic released, measurement window over, no verdict yet | an impact capability | review resumes with the verdict: record what it showed under `Success Evidence`, then decide the status |
| no match | none | report what was observed |
