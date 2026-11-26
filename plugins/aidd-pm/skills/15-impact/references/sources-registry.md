# Sources registry

The sources registry is the `sources` file of project memory, found where the memory block of the project's AI context file lists it, else at `aidd_docs/memory/sources.md`. It lists where product evidence can be read. This skill reads it and never creates or edits it.

| Column read | Used for |
| --- | --- |
| Category | matching the signal to a kind of source, such as `analytics` for usage or `billing` for revenue |
| Source | the tool to read, as the team names it |
| Access | how to read it: `mcp` or `cli` directly, `web` from public pages through a web reading tool, `export` by request, `manual` from figures the user supplies, `none` not at all |
| Can support | whether this source can establish the signal |
| Owner | the role to ask for an export or an access |

| Situation | Handling |
| --- | --- |
| registry absent | say so; offer Research plan to declare sources, one-way, or manual mode |
| no row can support the signal | offer Research plan or manual mode |
| matching row with access `none` | name the missing access and its owner; offer manual mode |
| access `export` | prepare the request for the owner; the reading stays pending until it arrives |
| manual mode accepted | take the figures the user supplies and note the mode in the report |
| manual mode refused | stop; nothing is measured |
