# Watchlist

The watchlist is the set of `market` rows in the sources registry: the `sources` file of project memory, found where the memory block of the project's AI context file lists it, else at `aidd_docs/memory/sources.md`. Research plan owns and creates that registry; this skill only reads it.

| Registry column | Read as |
| --- | --- |
| Category | `market` rows only; every other category is ignored |
| Source | the competitor, host platform, or market source, with the pages to read; a host platform is marked `host:` before its name |
| Access | `web`, `mcp`, or `cli` means the agent reads; `export` or `manual` means the user supplies; `none` means skipped |
| Can support | what the source can show: public claims, offers, prices |
| Owner | the role to ask when a source cannot be read |

| Situation | Handling |
| --- | --- |
| registry missing or without a `market` row | offer Research plan, which produces watchlists, or take a list from the user |
| competitors listed by the user | used for this run only; the registry stays untouched |
| host platform, the platform the product runs on or is distributed through, such as an IDE or a marketplace | read and journaled like a competitor, never counted as one |
| unclear whether a listed source is a competitor or a host platform | ask the user before scanning |
| competitor journaled, registry present, no longer in its `market` rows | no longer watched; never read again |
| competitor journaled but absent from a list given for this run | not read in this run; still watched |
| theme brought by the user | only observations touching that theme can raise a finding |
| no theme brought | the themes of the existing insights registry files, plus any new theme the user approves |

| Last read | Value |
| --- | --- |
| of a competitor | the latest dated entry or line in its own journal |
| of a source | the latest entry of its competitor's journal that does not list it as skipped |
| no journal yet | first run for that competitor; nothing to compare against |
| next due date | the last read plus the cadence in force per `practices.md` |
