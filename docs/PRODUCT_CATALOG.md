# A structured product catalog within SharePoint

**Workstream two · A master list and web parts used by staff**

The product catalog provided a consistent entry point into product information and its associated documents. I developed the master SharePoint list and the web parts used to present it. Staff used both the list and the product-page interface.

## Keep the record and its presentation connected

Structured records supplied the product information. The interface used SharePoint Framework, React, and TypeScript to retrieve and display those records within SharePoint. Document references remained connected to the relevant product.

<figure class="workflow"><ol class="process-flow"><li><span class="step-label">01</span><strong>Master list</strong><span>Maintain structured product information.</span></li><li><span class="step-label">02</span><strong>Browse</strong><span>Filter the catalog and open a product.</span></li><li><span class="step-label">03</span><strong>Read</strong><span>Present details in consistent sections.</span></li><li><span class="step-label">04</span><strong>Follow sources</strong><span>Open the associated documents.</span></li></ol><figcaption>A simplified reading workflow; no employer records, field definitions, or product rules are shown.</figcaption></figure>

This structure allowed the same underlying record to support a short gallery view and a more detailed product page. It also made browsing and filtering possible without asking users to open every product individually.

## Support a short path from browsing to detail

The implemented interface included a card-based gallery, filters, a product detail view, and separate areas for overview information and documents. Collapsible sections helped organize longer detail pages. Expand-all and collapse-all controls gave users a way to change how much information was visible.

The document interface handled different file types and links. It included preview fallbacks when a thumbnail could not be shown and handling for shortcut files that pointed to another location. Those details mattered because a catalog needs to take a user to the source document as well as display a summary of the product.

## Make the information structure usable

The master list and the interface served related purposes. The list organized product records into a consistent structure. The web parts turned those records into a reading and navigation experience for staff.

The catalog also provided a concrete direction for the wider intranet work: product information could be presented through a shared entry point while retaining links to its supporting material. Decisions about the meaning, currency, and ownership of that material remained with the business.

## Describe the implemented scope accurately

| Implemented in the reviewed work | Status in this case study |
|---|---|
| Master product list and SharePoint web parts | Used by staff |
| Gallery, filters, and detail views | Present in the implementation |
| Document links, previews, and collapsible sections | Present in the implementation |
| Further layout editing and richer authoring controls | Development ideas; not represented as delivered features |
| Copilot Studio product search | A later objective, separate from the staff-used catalog |

The report does not reproduce the underlying product definitions or describe the catalog as an automated lending-decision system. It presents the organizational and interface work at a level that can be discussed without disclosing the employer’s information.

[Return to the case study](../README.md) · [Content review workstream](CONTENT_REVIEW.md)
