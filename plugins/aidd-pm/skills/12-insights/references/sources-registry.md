# Sources registry

The sources registry is the `sources` file of project memory, found where the memory block of the project's AI context file lists it, else at `aidd_docs/memory/sources.md`. It lists where product evidence can be read. Its columns are Category, Source, Access, Can support, and Owner. This skill only reads it.

| Access | How signals are read |
| --- | --- |
| `mcp` | through the connected tool, filtered to the scope period and theme |
| `cli` | through the declared command line tool, filtered the same way |
| `web` | from public pages, opened with a web reading tool and filtered to the scope period |
| `export` | from the export file the user points to; ask for it when none is pointed |
| `manual` | from the material the user supplies |
| `none` | unreadable; an export is asked of the Owner role |

| Situation | Handling |
| --- | --- |
| registry missing | never create it; it belongs to Research plan |
| category whose source is `none` | nothing to read; report the gap |
| declared access fails at read time | unreadable for this run; the registry unchanged |
| source the registry does not declare | read it in manual mode and suggest declaring it through Research plan |
| any row | read as written; never infer an endpoint or a credential |
