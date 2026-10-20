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

## 3. Any agent position may be made a human seat by its manager

- **Current text.** The Standard and the Protocol name each Cell's filler kind (`human` or `ai`) on its card; no clause says who may change it, or how.
- **Proposed text.** Add to the Protocol: "The manager of any AI Cell (the seat it is accountable to) may make it a human seat, a HOAC named by the position, for a period or for good, and may turn it back. The Cell keeps its code, card, duties and independence rules; its filler kind changes by an entry in the unit register, which the human hub writes the same day with the person who stands behind it. A human seat has its own Chief of Staff; by default, the AI Cell that held the position." Add a matching line to the AIOC template's section on Cells and Pods.
- **Reason and evidence.** An organisation run almost wholly by agents must be able to bring people in wherever judgement, trust or a relationship needs them, at any time, and step back again, without redesigning a part. The first instance's governing seat asked for it for the whole of its `[ORG]AION` (`MANDATE.md` §4.6).
- **Parts and tests affected.** The Standard (Cells and Pods); the Protocol (the unit register); the AIOC template; each part's fixed test gains a case: a Cell made human keeps its card and its independence rules.

## 4. A human seat may hand its acts to its own Chief of Staff

- **Current text.** The Standard keeps decisions, acceptances and signatures under a human seat's credential (Human Floor); the Product Core mother kept its reserved acts from every agent (blueprint 3, TEST-PC v1, case 42).
- **Proposed text.** Add: "A human seat may hand any of its work or decisions to its own Chief of Staff, on its own responsibility, by a delegation it signs: what is handed, its limits and its term. Each act taken under it is recorded as the seat's own act, naming the delegation; the Chief of Staff never signs in its own name. What the law, a regulator or the source of record gives to a natural person, and a two-person control, stay with people. Every human act has a default time and a stand-in; nothing approves itself."
- **Reason and evidence.** A seat that cannot hand its decisions becomes the queue of its own team; the record keeps the decision the person's, made in advance, as standing rules already do (`MANDATE.md` §4.3, §4.4).
- **Parts and tests affected.** The Standard (Human Floor wording, if it reads as forbidding delegation); the Protocol (standing rules and delegations); TEST-PC (cases for delegation, stand-ins and the record).

*Powered by 49GAION*
