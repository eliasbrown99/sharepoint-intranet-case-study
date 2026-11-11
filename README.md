# Organizing an intranet around the people who use it

**Elias Brown · SharePoint, Python, information architecture, and React · An anonymized employment case study**

At a mortgage lender, I worked on how information should be organized across the intranet. The practical questions were where a loan officer should look for a product document, which version should be treated as current, and whether related material belonged together or across separate sites.

I built a content inventory and knowledge graph to make the existing structure easier to examine. I used that work in discussions with underwriters, loan officers, and operations staff to identify outdated, redundant, or inappropriately placed material and begin a SharePoint cleanup. I also developed a master product list and SharePoint web parts that staff used to browse product information and its associated documents.

## What the work produced

| Workstream | Deliverable | Use and status |
|---|---|---|
| Intranet content review | A content inventory, relationship graph, and review reports | Used to inform cross-department discussions and begin cleanup |
| Product information | A master SharePoint list and product web parts | Used by staff to access product information and documents |
| Search exploration | Working custom integration and search prototypes | Explored a path toward later AI-enabled product search; a completed Copilot Studio rollout is not claimed |

The established outcomes are the tools, their use in staff discussions, and staff use of the product interface. This case study does not attach a measured time saving or a completion percentage to the cleanup.

## Start with the organization of the information

A search tool can retrieve material from several locations without resolving which copy is authoritative or where a user would expect it to live. The content review therefore examined the organization around the documents as well as the documents themselves.

<figure class="workflow"><ol class="process-flow"><li><span class="step-label">01</span><strong>Inventory</strong><span>Understand the material and where it lives.</span></li><li><span class="step-label">02</span><strong>Map</strong><span>Connect pages, documents, lists, and navigation.</span></li><li><span class="step-label">03</span><strong>Discuss</strong><span>Review placement and authority with staff.</span></li><li><span class="step-label">04</span><strong>Organize</strong><span>Support cleanup and a structured product catalog.</span></li></ol><figcaption>Generalized account of the work. This is not a reproduction of the employer’s intranet, data, or site map.</figcaption></figure>

The inventory and graph offered complementary views. Metadata helped locate related filenames and possible version conflicts. Links showed how people could move between pages, documents, and sites. Together, they gave staff concrete material to discuss when considering a different structure.

[How the content review worked](docs/CONTENT_REVIEW.md)

## Turn the findings into questions staff could answer

The review tools developed beyond lists of technical flags. A later reporting approach framed findings as questions about why content was scattered, which location should own it, and whether additional sites made navigation easier or harder.

This was useful for discussions with people who understood the material and used it in their daily work. A matching filename could suggest duplication; it could not decide whether two departments needed different versions. A document’s modification date could guide review; it could not establish that the guidance was still valid. Those decisions needed business context.

The resulting direction was to make current information easier to identify, give related content a coherent home, and provide a clearer way to reach product information. The work began a cleanup process; the report does not represent every proposed restructuring action as completed.

## Give product information a consistent entry point

The second workstream put structured product information into a master SharePoint list and presented it through custom web parts. Staff could browse a gallery, narrow the results, read a product’s details, and follow links to associated documents.

This connected the organization work to an interface people could use. The report describes the catalog’s structure and behavior without reproducing any loan product, underwriting rule, internal field schema, or company screenshot.

[How the product catalog worked](docs/PRODUCT_CATALOG.md)

## My contribution

I was the sole contributor to the two underlying projects. My work covered the technical implementation and the use of the content map to support discussions about intranet organization. Underwriters, loan officers, and operations staff supplied the operational context for those discussions. The product web parts and master list were used by staff; the integration and search work included working prototypes.

The original implementation used custom integrations built with the tools available to the project at the time. AI-enabled search through Copilot Studio was a later objective. The experience is relevant both to building internal tools and to deciding what information those tools should expose.

## Scope of this account

The employer is described only as a mortgage lender. All diagrams are newly authored, generalized explanations. Internal content, site names, URLs, schemas, screenshots, source code, resource identifiers, and operational records remain private. No live connection to the employer’s systems is part of this report.
