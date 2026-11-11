# Making intranet structure visible and reviewable

**Workstream one · Content inventory, relationship mapping, and restructuring discussions**

The central question was how to organize the intranet so that loan officers and departments could reach appropriate, current information. To discuss that question concretely, I needed a view of both where content was stored and how it was connected.

## Use metadata for the first pass

The metadata-analysis tool inspected document names, locations, modification dates, sizes, and related properties without downloading document bodies. This supported an initial structural review before full content ingestion.

The approach was appropriate to the question: identifying material that might be duplicated or placed inconsistently did not always require reading every file. The repository also contains ingestion tools for documents, pages, and lists, but metadata review could be carried out separately.

| Signal | Question it helped raise | Boundary of the signal |
|---|---|---|
| Related filenames across locations | Are several locations maintaining copies of the same material? | Name similarity is not proof of identical content |
| Apparent versions and modification dates | Which copies need a currency or archiving review? | The most recently modified file is not automatically authoritative |
| Related subjects spread across sites | Does the arrangement match how staff look for the material? | Similar subject matter does not necessarily require one owner or one site |
| Inconsistent naming and folder patterns | Is the organization understandable and maintainable? | Naming conventions alone do not determine correctness |

These were review signals, not automatic deletion instructions. The underlying rules could produce candidates for discussion, while content owners and users determined what those candidates meant.

## Map relationships as well as storage locations

The knowledge graph represented content as nodes and relationships as links. It connected sites, pages, documents, and lists so that navigation could be inspected across boundaries that a folder listing alone would not show.

The implementation extracted page links, distinguished types of references, normalized URLs, and grouped connections for visualization. An interactive graph made it possible to inspect clusters and cross-site connections. Potentially isolated material or unresolved references provided additional starting points for review.

A graph’s interpretation depends on what was included in the inventory. An unresolved reference might indicate an access or extraction limitation rather than a deleted page. A highly connected page might be a useful navigation hub, but its number of links would not establish the accuracy of its content.

## Develop a review conversation

The restructuring tools examined content overlap, folder proliferation, and placement. A later version generated a question-based review report: why was related information spread across locations, what distinguished the copies, and which structure would make sense to the people using it?

That reporting approach supported the discussions I held with underwriting, loan officers, and operations. It helped move from an observation about files or links to a conversation about information ownership, navigation, and the intended use of the intranet.

The accompanying review-report interface also supported checkboxes and notes. Those controls stored state in the reviewer’s browser; they were not a shared workflow database. The useful artifact was a reviewable set of issues and questions, not a claim that multi-user remediation tracking had been implemented.

## Separate a proposed structure from a completed change

The work informed a cleanup effort and a more structured approach to product information. Proposals to consolidate content, distinguish current material from older copies, or change a navigation route still required a decision from the people responsible for the information.

This account reports the use of the analysis to begin that work. It does not include a migration completion rate, a measured reduction in obsolete material, or a verified search-quality benchmark. Numerical examples in development documentation are not used as evidence of business impact.

## Put the custom integration in context

The original work included working prototypes built through explicit content extraction, relationship mapping, and search configuration. The choices reflected the tools available to the project at that time.

As of November 2026, Microsoft documents built-in ways to [add SharePoint knowledge to Copilot Studio](https://learn.microsoft.com/en-us/microsoft-copilot-studio/knowledge-add-sharepoint) and [connect an agent to an MCP server](https://learn.microsoft.com/en-us/microsoft-copilot-studio/mcp-add-existing-server-to-agent). Those capabilities suggest that some connection and orchestration work could be simpler in a new implementation. The original project used custom integrations in its own working environment; this comparison describes how I would assess the approach today.

The organizational questions would still need answers: which source is authoritative, what belongs together, who maintains it, and whether staff can find it. The work documented here addressed those questions while developing a path toward later AI-enabled search.

[Return to the case study](../README.md) · [Product catalog workstream](PRODUCT_CATALOG.md)
