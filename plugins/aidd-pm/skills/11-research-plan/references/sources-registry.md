# Sources registry

The sources registry is the `sources` file of project memory, found where the memory block of the project's AI context file lists it, else at `aidd_docs/memory/sources.md`. It declares where product evidence can come from; created at that default, it is wired into the AI context files like the rest of the bank.

| Column | Holds |
| --- | --- |
| Category | `analytics`, `support`, `interviews`, `surveys`, `billing`, `sales`, `market`, or a project category |
| Source | the tool or channel as the team names it, or `none` |
| Access | `mcp`, `cli`, `web` for public pages an agent reads with a web reading tool, `export`, `manual`, or `none` |
| Can support | what this source can establish, per `coverage.md` |
| Owner | the role that can grant access or run a collection |

| Situation | Handling |
| --- | --- |
| registry missing | propose rows from project memory and visible integrations, ask for the rest |
| category with no source | keep the row with source `none`; it is a known gap |
| source named, nobody can read it yet | keep it with access `none` until the user names one |
| tool name only | record it as declared; never infer an integration or an endpoint |
| market source that is the platform the product runs on or ships through | a `market` row whose Source starts with `host:` |
| row added or changed | change only the approved rows; keep every other line |
