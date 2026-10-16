# Drafts of proposals to 49GAION

**49GAION Product Core, mother blueprint `v0.1.0` · 16 October 2026.** Drafts only. Nothing here is proposed to 49GAION without the word of its governing seat; then only by pull request, merged by that seat. Each draft is generalised: no organisation's name or data.

## 1. A Library contract for the product package

- **Current text.** Protocol §18, item 10: "Product work reaches the engineering AIOC only as complete product packages, on the product line between the two parts." The part card names the format "frozen, content-addressed package (manifest + parts by hash)". No Library contract gives its fields.
- **Proposed text.** Add `library/contracts/product-package.schema.json`, with valid and must-fail examples: the manifest of blueprint Annex A.1 (`package_id` as the hash of the canonical manifest; parts by hash; the acceptance index; `rests_on`; `decided_by`), and the notices of the line (question, first-look build, acceptance request, answer, acceptance), each citing the package by `package_id`.
- **Reason and evidence.** Without a contract, each organisation's Product Core and engineering AIOC would invent their own package shape, and the product line could not be tested across parts (TEST-PRODUCT-CORE v1, case 11).
- **Parts and tests affected.** Protocol §18, item 10; the engineering part's card; TEST-PRODUCT-CORE (a case for the contract's fixtures).

## 2. Product documents in Source Lifecycle

- **Current text.** Protocol §18 and the part card: explainers and supporting documents are "filed into Source Lifecycle as sources". Source Lifecycle's origin kinds name the design stages' filings only.
- **Proposed text.** Either read the filing as an ordinary source from the product's owner position as contributor (no change), or add an origin kind `product document`, filed only by `[ORG]AIOC-PC`, with its own write scope.
- **Reason and evidence.** A retirement withdraws a product's documents (blueprint §5.10); a kind of their own lets Source Lifecycle find and withdraw them as a set.
- **Parts and tests affected.** Protocol §13; the Source Lifecycle card; TEST-SOURCE-LIFECYCLE.

*Powered by 49GAION*
