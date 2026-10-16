```yaml
# ── Blueprint metadata (machine-readable; the panel generator and the back-office builder read this block) ──
blueprint:
  aioc: "[ORG]AIOC-PC"
  parent: "[ORG]AIOC-CH"                  # example code of the Charter; each organisation writes its own Charter's code (Standard §1.7, item 13)
  full_name: "Product Core"
  organisation: "<organisation>"          # filled in each organisation's own copy
  type: "structural"
  org_aion: "[ORG]AION"
  blueprint_version: "v0.1.0"
  status: "draft"
  template:
    name: "49GAION AIOC Blueprint Template"
    version: "v1.5.0, with the unreleased v1.6.0 additions on main"
    source: "github.com/49g-holding/49GAION-aioc, template/AIOC-BLUEPRINT-TEMPLATE.md @ 1abae80"
  mother:
    name: "49GAION Product Core"
    version: "part card v1 (DRAFT)"
    source: "github.com/49g-holding/49GAION-protocol, library/cards/product-core.part-card.json and the Protocol section Product Core (§18) @ db682c4. This text is its mother blueprint, in its mother repository github.com/49g-holding/49GAION-product-core (49GAION DR-0024)"
  writing_repository: "<org>aioc-pc"
  code_project: "none: Product Core writes no code (Protocol §18, item 6.4)"
  panel_register_id: "none yet"
  capabilities:
    standard: ["Chief of Staff", "Office", "Input socket", "Panel"]
    functional: ["Product Intake", "Portfolio and Categories", "Research and Opportunity", "PRD and Feature Packages", "Design", "Partnership in Build", "Launch", "Run", "Explainers and Supporting Documents", "Product Review, Refresh or Retire", "Shared Standards"]
```

# Blueprint · `[ORG]AIOC-PC` · Product Core · `v0.1.0`

**Draft, 16 October 2026.** The mother blueprint of the Library part 49GAION Product Core, for any organisation (`49GAION/DR-0024`; `decisions/DR-0001`). It sets the structure stated in the Protocol section Product Core (§18) and the part card `product-core.part-card.json` v1 into the form of the 49GAION AIOC template: its card, its positions, its Cells and Pods, and each capability in four parts. Every rule rests on a 49GAION text, cited by section, or is new in this blueprint and marked **New**. It holds no organisation's data: no product, no category, no price, no company. Each organisation fills its own copy (§0, §2.1). Nothing here has run. Every fixed test reads `NOT_RUN`.

> **Product Core in one page**
>
> Product Core is the organisation's one product division, shared by every company the organisation runs. It is to products what the organisation's engineering AIOC is to engineering (Protocol §18, item 1).
>
> **What it owns.** The what and the why of every product, across the product's whole life: design, the partnership in build, and the run. The engineering AIOC owns the how and the when (item 2).
>
> **Its head office** is the CPO Office. Every product owner reports to it. It holds the intake of product work, the portfolio of products and their categories, the shared standards, the weekly product review, and the line to the engineering AIOC. Its accountable seat is a human position, the Chief Product Officer (item 3).
>
> **One product, one team.** Products are split small. Each product has one team for every stage of its life, and the team stays with it: one owner position whose only job is that product, and AI members by function (item 5). Each team goes, in order, through:
> 1. research and opportunity;
> 2. the PRD and its feature packages, with acceptance criteria;
> 3. design: flows, a screen for every state, copy in every language the product serves;
> 4. partnership in build: answers, first look, acceptance criterion by criterion; never code;
> 5. launch;
> 6. run: pricing and rates, performance and profit and loss, communications and retention, customer voice and complaints, operations;
> 7. explainers and supporting documents;
> 8. refresh or retire.
>
> **What it never does.** It writes no code and no technical design, speaks to no builder and no code host, copies no product per company, records no capability as a product, and names no person. Rates are versioned data, never a code release (items 6 to 11).

**Where this blueprint stands.** No instance has run. The part card is `DRAFT`, with `last_result` `NOT_RUN` (Protocol §18, item 12). The product line to the engineering AIOC has no Library contract yet; Annex A gives its field lists, and a contract is drafted upstream (`upstream/PROPOSALS.md`, item 1). The decisions only a human seat can take are listed once, in §13.

---

## 0. Identity and lineage

| Field | Value |
|---|---|
| Code | `[ORG]AIOC-PC`. Collision check (Naming Standard §5): the initials do not recreate `AIOC`, `AION` or `49GAION`, and do not read as a version suffix. The code is the one Protocol §18 gives the Library part in an `[ORG]AION`. Each organisation records it in its register before its repository is created (Naming Standard R9) |
| Full name | Product Core |
| Description | "`[ORG]AIOC-PC` is `<organisation>`'s Product Core, built from 49GAION Product Core" |
| Kind | AIOC |
| Parent | `<code of the Charter of this [ORG]AION>`; the cards use the example code `[ORG]AIOC-CH`. A top-level AIOC: only the Charter has parent `none` (Standard §1.7, item 13). Like every other part, it enters through OCO (Protocol §18, item 1). A change of parent is the listed type `change-parent` |
| Inner units | `[ORG]CELL-CPO`, `[ORG]CELL-PCCS`, `[ORG]POD-PCCO` (the CPO Office), and one product team Pod per product, made from the pattern `[ORG]POD-EPT` (§17). No inner AIOC |
| HOAC label | `[ORG]HOAC-ACS`, held by its top Cell, the Chief Product Officer `[ORG]CELL-CPO` (`label_holder`) |
| Accountable to | `<code of the Cell carrying [ORG]HOAC-TM>`; the cards use the example code `[ORG]CELL-TMS` (Naming Standard R15). That Cell signs this AIOC's install, its `change-parent` and its `restart-stopped-unit` (Standard §5.3, item 4; §4.4, item 3) |
| Type | Structural: it is the organisation's product division (§16) |
| `[ORG]AION` | `[ORG]AION`, based on 49GAION Standard `v1.5.0`, with the unreleased `v1.6.0` texts on main |
| Versioned Definition | this file; the Panel and the Back office are built from it |
| Organisation | `<organisation>` |
| Made from | the Library part 49GAION Product Core, part card `v1` (DRAFT), and the Protocol section of the same name (§18), proposed on 15 October 2026 |
| Template | 49GAION AIOC Blueprint Template `v1.5.0` at `1abae80`, with the unreleased `v1.6.0` additions |
| Mother | 49GAION Product Core, part card `v1`. This text is its mother blueprint, held in the part's mother repository `github.com/49g-holding/49GAION-product-core` and pinned in the Library register (`49GAION/DR-0024`) |
| Blueprint version and status | `v0.1.0` · draft |
| Accountable seat (`[ORG]HOAC-ACS`) | the Chief Product Officer position, `[ORG]CELL-CPO`. Who occupies it is top management's own mechanism (Standard §1.1, item 9; §5.2, Position Principle) |
| Reports to | the Cell carrying `[ORG]HOAC-TM` |
| Writing repository | `<org>aioc-pc`, private where it holds the organisation's products, categories and rates, plus `-records` for the AIOC's run records and `-records-restricted` for records that touch personal data (Naming Standard R9) |
| Code project | none: Product Core writes no code and no technical design (Protocol §18, item 6.4) |
| Panel | not yet built (§4.4) |
| Back office | not yet built |
| Attribution | Powered by 49GAION |

**Lineage.** The part was stated by the governing seat of 49GAION on 15 October 2026 as the organisation's one product division (Protocol §18), from a first organisation's need for one home for the what and the why of every product, apart from engineering. This is its first blueprint. Its mother lives in its own public repository because the first instance's home holds that organisation's products and categories (`49GAION/DR-0024`).

---

## 1. Card (49GAION Operating Protocol §3)

```yaml
card:
  unit_kind: "AIOC"
  code: "[ORG]AIOC-PC"
  parent: "[ORG]AIOC-CH"                  # example code of the Charter, the root AIOC; only it has parent none (Standard §1.7, item 13)
  inner_units: ["[ORG]CELL-CPO", "[ORG]CELL-PCCS", "[ORG]POD-PCCO", "[ORG]POD-EPT"]
  type: "structural"
  org_aion: "[ORG]AION"
  card_version: "v0.1.0"
  input_door: "Chief of Staff"
  wake: { method: "queue", verified: false }
  receives:
    - kind: "product request"             # product direction and product requests, from the Requesting Authority's Cell and from a position of each company, through the HU input port; references only
      format: "Work Item (ID + version) naming the requesting position, the company or market it is for, and what is asked; sources by reference"
      acceptance_test: "TEST-PC v1, cases 2, 14, 15"
      decision_needed: false
    - kind: "source reference"            # the organisation's sources (product documents, terms, policies, data), from the output socket of [ORG]AIOC-SL
      format: "source reference (ID + version + hash; held or not held)"
      acceptance_test: "TEST-PC v1, cases 16, 22"
      decision_needed: false
    - kind: "product signal"              # performance, customer voice, complaints and support, from products in use, through the tool gateway
      format: "Work Item or record reference (ID + version)"
      acceptance_test: "TEST-PC v1, cases 31, 32"
      decision_needed: false
    - kind: "engineering request"         # a question, a first-look build or an acceptance request from the engineering AIOC, on the product line
      format: "Work Item (ID + version) citing the product package (manifest hash) and the criterion it concerns"
      acceptance_test: "TEST-PC v1, cases 11, 27, 28"
      decision_needed: false
    - kind: "rate record"                 # the read-back of a rate written to the rate and configuration store
      format: "versioned record (ID + version), read back"
      acceptance_test: "TEST-PC v1, case 8"
      decision_needed: false
  delivers:
    - kind: "product package"             # the PRD, feature packages with acceptance criteria, designs for every state and copy in every language, on the product line
      format: "frozen, content-addressed package (manifest + parts by hash; Annex A)"
      usual_receivers: ["<code of the engineering AIOC>"]
    - kind: "answer or acceptance"
      format: "Work Item (ID + version): an answer to a question, a first-look note, or an acceptance criterion by criterion"
      usual_receivers: ["<code of the engineering AIOC>"]
    - kind: "rate record"
      format: "versioned record (ID + version) with its effective date, its reason and the record it replaces (Annex B)"
      usual_receivers: ["the rate and configuration store"]
    - kind: "explainer filing"
      format: "versioned document (explainer, questions and answers, help article, user guide, partner material, internal training), filed into Source Lifecycle as a source"
      usual_receivers: ["[ORG]AIOC-SL"]
    - kind: "product review outcome"
      format: "Work Item (ID + version): keep, fix, grow or retire, with its evidence"
      usual_receivers: ["the Requesting Authority's Cell"]
  anatomy:
    panel: { health: { tests: true, metrics: ["stuck", "returned", "late", "products by stage", "packages refused by the auditor", "questions open from engineering", "acceptances open", "rates changed", "rates reversed", "explainers missing", "reviews held"] } }
    back_office: { converses_with_humans: true, hosts: ["Chief of Staff", "Office"], protocol_traffic: true }
    definition: { location: "<org>aioc-pc, blueprint/PC-BLUEPRINT.md", version: "v0.1.0" }
    delivery: { rollback: "one-click" }
    connectors:
      - { role: "the product line to the engineering AIOC", connector: "<engineering AIOC> product line port", access_managed_in: "panel" }   # the grant is signed at the tool gateway as connect-external-port
      - { role: "source of record", connector: "[ORG]AIOC-SL output socket", access_managed_in: "panel" }
      - { role: "rate and configuration store (versioned)", connector: "<store>", access_managed_in: "panel" }
      - { role: "product signals", connector: "<signal source>", access_managed_in: "panel" }
    gateway: { metering_id: "<per-AIOC metering id>" }
  full_name: "Product Core"
  version: "0.1.0"
  lineage: { id: "[ORG]AIOC-PC", version: "0.1.0", relation: "original" }
  lifecycle_state: "designed"
  blueprint_version: "v0.1.0"
  template_version: "v1.5.0"
  accountable_to: "[ORG]CELL-TMS"         # example code of the Cell carrying [ORG]HOAC-TM (Naming Standard R15); never a Cell inside this AIOC
  top_cell: "[ORG]CELL-CPO"
  hoac: "[ORG]HOAC-ACS"
  label_holder: "[ORG]CELL-CPO"
  fixed_test: { id: "TEST-PC", version: "v1", owner: "[ORG]CELL-TMS" }
  skills:
    - { id: "pc-intake", name: "Product intake: the what and the why, apart from the how and the when", tags: ["product", "intake"] }
    - { id: "pc-portfolio", name: "The portfolio of products and their categories", tags: ["product", "portfolio"] }
    - { id: "pc-prd", name: "PRDs and feature packages with acceptance criteria", tags: ["product", "requirements"] }
    - { id: "pc-design", name: "Product design: flows, every state, copy in every language", tags: ["product", "design"] }
    - { id: "pc-build-partner", name: "Partnership in build: answers, first look, acceptance", tags: ["product", "build"] }
    - { id: "pc-run", name: "The run: rates as data, performance, customer voice", tags: ["product", "run"] }
    - { id: "pc-explainers", name: "Explainers and supporting documents", tags: ["product", "documents"] }
    - { id: "pc-review", name: "The weekly product review; refresh or retire", tags: ["product", "review"] }
  ports:
    - { unit: "[ORG]AIOC-PC", port: "ai-in", direction: "input", type: "AI", identification: "technical-key", accepted_content: ["source reference", "product signal", "engineering request", "rate record"], authority_limit: "read only, within the scopes signed for each connection; requests on the product line only", audit_trail: "unit register; the serve logs of [ORG]AIOC-SL and of the engineering AIOC", required_tests: ["TEST-PC v1"], enforcement: "shared-gateway-outside-unit" }
    - { unit: "[ORG]AIOC-PC", port: "ai-out", direction: "output", type: "AI", identification: "technical-key", accepted_content: ["product package", "answer or acceptance", "rate record", "explainer filing", "product review outcome"], authority_limit: "packages, answers and acceptances on the product line only; rate records signed by the product's owner position; filings of its own documents only; never code, technical design or an instruction to a builder", audit_trail: "Work Item record and the unit register", required_tests: ["TEST-PC v1"], enforcement: "shared-gateway-outside-unit" }
    - { unit: "[ORG]AIOC-PC", port: "hu-in", direction: "input", type: "HU", identification: "live-human-sign-in-at-gateway", accepted_content: ["product request from the Requesting Authority's Cell or a company's position (references only)", "a decision of the Chief Product Officer or of a product owner position", "run control and configuration from the Chief Product Officer (never a source)"], authority_limit: "the signer's authority_scope; nothing received here is a source", audit_trail: "Office record", required_tests: ["TEST-PC v1"], enforcement: "shared-gateway-outside-unit" }
    - { unit: "[ORG]AIOC-PC", port: "hu-out", direction: "output", type: "HU", identification: "live-human-sign-in-at-gateway", accepted_content: ["review brief to the Chief Product Officer", "decision rows to the owner positions", "product review outcome to the Requesting Authority's Cell"], authority_limit: "information and proposals only; never a decision, an instruction or a question about a person", audit_trail: "Office record", required_tests: ["TEST-PC v1"], enforcement: "shared-gateway-outside-unit" }
    - { unit: "[ORG]AIOC-PC", port: "stop", direction: "input", type: "HU", identification: "live-human-sign-in-at-gateway", accepted_content: ["stop"], authority_limit: "stop only", audit_trail: "unit register", required_tests: ["TEST-PC v1"], enforcement: "shared-gateway-outside-unit", stop_door: true }
  configuration:                          # every slot is set by the organisation (§15); an empty slot fails the joining test
    office_accountable_human: { value: "<set by the organisation>", set_by: "<position>", date: "<date>", version: "<vN>" }
    central_head: { value: "<the OCO of this [ORG]AION>", set_by: "<position>", date: "<date>", version: "<vN>" }
    discussion_limits: { value: "<set by the organisation>", set_by: "<position>", date: "<date>", version: "<vN>" }
    waiting_deadlines: { value: "<per status>", set_by: "<Cell carrying [ORG]HOAC-TM>", date: "<date>", version: "<vN>" }
    bounce_limit: { value: "<number>", set_by: "<position>", date: "<date>", version: "<vN>" }
    chain_depth: { value: "<number, at least 1>", set_by: "<position>", date: "<date>", version: "<vN>" }
    halt_request_priority: { value: "immediate", set_by: "<position>", date: "<date>", version: "<vN>" }
    budget_cap: { value: "<amount per period>", set_by: "<Cell carrying [ORG]HOAC-TM>", date: "<date>", version: "<vN>" }
    unattended_action: "read-record-triage"
    requesting_authority_cell: { value: "<set by the organisation>", set_by: "<Cell carrying [ORG]HOAC-GOV>", date: "<date>", version: "<vN>" }
    engineering_aioc: { value: "<code of the organisation's engineering AIOC>", set_by: "<Cell carrying [ORG]HOAC-TM>", date: "<date>", version: "<vN>" }
    categories_record: { value: "<reference to the organisation's own category record; never in the Library>", set_by: "[ORG]CELL-CPO", date: "<date>", version: "<vN>" }
    review_day: { value: "<weekday of the weekly product review>", set_by: "[ORG]CELL-CPO", date: "<date>", version: "<vN>" }
    rate_signers: { value: "<per product: the owner position; and whether a rate change is also commit-money, with its limits (§13, H-03)>", set_by: "<Cell carrying [ORG]HOAC-TM>", date: "<date>", version: "<vN>" }
    audit_families_min: { value: 2, set_by: "<position>", date: "<date>", version: "<vN>" }
```

**Joining the protocol.** This AIOC joins only after every input and output on this card passes fixed samples (the joining test, Protocol §11, item 1; Standard §3.2, item 4). It also needs the engineering AIOC to accept product packages only on the product line and to send its questions, first looks and acceptance requests back on it, and Source Lifecycle to accept its documents as sources. Until then its `lifecycle_state` stays `designed` and no Work Item is routed to it. The cards of its Pods and Cells are set in §17 and generated into `cards/`.

---

## 2. Organisation table and placement

### 2.1 Organisation table

The blueprint writes `[ORG]` for the organisation's prefix, as central texts do (Naming Standard R13); each organisation fills it in its own copy. Positions only; who holds each one is kept only in the private register copy (Standard §5.2, Position Principle; `49GAION/DR-0011`).

| Term in the blueprint | In `<organisation>` |
|---|---|
| The Top Office (decisions are signed by human Cells carrying HOAC labels) | `<filled by the organisation>`, the human hub |
| `[ORG]AIOC-OCO` | `<filled>` |
| The Charter of this `[ORG]AION` | `<code>`; the cards use the example code `[ORG]AIOC-CH` |
| The Cell carrying `[ORG]HOAC-TM` | `<code>`; the cards use the example code `[ORG]CELL-TMS` |
| **The Requesting Authority**: the seat that gives product direction and decides what the organisation offers | `<code of the human Cell carrying [ORG]HOAC-GOV>`, or of a human Cell whose `authority_scope`, delegated by that Cell under `delegate-authority`, covers product direction |
| **The engineering AIOC**: the part that owns the how and the when of building | `<code>`; the other end of the product line (Protocol §18, item 10) |
| The IT and infrastructure division | `<filled>` (the rate and configuration store's hosting, the tool gateway's hosting) |
| The builder of every tool | `<filled>` |
| **The source of record** | `[ORG]AIOC-SL`: every source this AIOC reads comes from its output socket, by reference; every explainer and supporting document is filed into it (Protocol §13) |
| **The companies and markets** the organisation's products are offered in | the organisation's own record, by reference; never in this file |
| **The product categories** | the organisation's own record (Protocol §18, item 4), by reference in slot `categories_record` (§15); never in the Library |
| The Library blueprint this core is made from | 49GAION Product Core, part card `v1` (DRAFT); Protocol §18; this text is its mother blueprint |

### 2.2 Placement

- **Where it sits.** A top-level AIOC under the Charter, accountable to the Cell carrying `[ORG]HOAC-TM`, beside the engineering AIOC (Protocol §18, item 1).
- **Its role.** The organisation's one product division: it owns the what and the why of every product for the product's whole life (item 2).
- **Scope: does.** Product intake; the portfolio and its categories; research; PRDs and feature packages; design; partnership in build; launch; the run (rates as data, performance and profit and loss, communications and retention, customer voice and complaints, operations and upkeep); explainers and supporting documents; refresh or retire; the shared standards of the part (items 3 to 8).
- **Scope: does not.** Code, technical design, infrastructure, the build plan or its dates (the engineering AIOC); a contract, a legal filing or a money commitment (Human Floor seats); the organisation's own sources (Source Lifecycle); any instruction to a builder (item 10).
- **Companies it serves.** Every company the organisation runs, and every market it offers in. A product is made once and configured for each company and market, never copied (item 9).
- **Boundaries with other AIOCs.**
  - **The engineering AIOC** holds the how and the when. The only line between the two is the product line: complete product packages go out; questions, first-look builds and acceptance requests come back. A finding in build that would change the product comes back as a question (item 10).
  - **Source Lifecycle** holds every source. This AIOC reads sources by reference and files its own documents into it as sources; it keeps no second copy (Protocol §13).
  - **The design stages** (Target Operating Model, Process and Position Design, Delivery and Implementation) design the organisation. Where a decided design places a capability or process in Product Core, this AIOC reads it by reference from Source Lifecycle; it never designs the organisation.
- **Overlap.** None by design. A product decision found elsewhere is returned to this AIOC; a how or when decision found here is returned to the engineering AIOC (TEST-PC v1, case 2).

---

## 3. Positions

Every human position is a HOAC position, a legal persona; no natural person exists in the system (Standard §1.1, item 9; `49GAION/DR-0013`, `DR-0015`). Two positions are two parties. Who occupies a position, and how, is top management's own mechanism, never in this file.

| Position (standard title) | Purpose | Reports to | Run today by | Deputy |
|---|---|---|---|---|
| Chief Product Officer (`[ORG]CELL-CPO`, `[ORG]HOAC-ACS`) | leads the CPO Office; accountable for every product and every product team; creates and retires product teams | the Cell carrying `[ORG]HOAC-TM` | a person (holders register) | an acting filler appointed under `appoint-acting-filler` |
| Product owner, one per product (pattern `[ORG]CELL-EPO`, `[ORG]HOAC-ACS`) | the only job is one product, for its whole life; decides that product's what and why, its stage moves, its acceptance and its rates | the Chief Product Officer | a person (holders register) | an acting filler appointed by the Chief Product Officer |
| Product Core Chief of Staff (`[ORG]CELL-PCCS`) | this AIOC's voice to its HOAC seats; the door of every input; holds the product line | the Chief Product Officer | an agent | the Chief Product Officer holds its work |
| The AI Cells of the CPO Office and of each product team (§17) | each performs one role card | the Chief Product Officer, or the team's product owner | an agent | its Pod's top Cell holds its work |

**One product, one owner** (Protocol §18, item 5). An owner position holds no other product; a product has exactly one owner position. A product with no owner position, or an owner position named for two products, fails (TEST-PC v1, cases 5, 48).

Each position's role pack is carried in the role cards of the capabilities it performs (§4, §5).

---

## 4. Standard capabilities

### 4.1 Office
#### Definition
Default (`49GAION-aioc` `docs/STANDARD-CAPABILITIES.md` §4.1) · form: single Chief of Staff. An Office is proposed to the Chief Product Officer when the queue exceeds the waiting deadlines for two review periods; it is never self-created.
#### Process (SOP)
Default.
#### Role card
Default; Performed by: an agent; Reports to: the Chief Product Officer.
#### Fixed test
TEST-PC v1, case 38 · result `NOT_RUN`

### 4.2 Chief of Staff
#### Definition
Default, with these additions. It is this AIOC's voice to its HOAC seats; input arrives only through the typed ports and the Input socket. It holds the product line: it sends only frozen packages that the Independent Package Auditor has passed, and it routes every question, first-look build and acceptance request from the engineering AIOC to the product's team. It writes no product content of its own.
#### Process (SOP)
| Field | Content |
|---|---|
| Trigger | a Work Item at any input port; a stage's done-test result; the review day; a waiting deadline reached |
| Steps | 1. CoS — read the item; record it; name its product, or open an intake record — intake record. 2. CoS — check the request's kind: a how or when matter goes back to the engineering AIOC with its reason (Protocol §18, item 2) — returned item. 3. CoS — dispatch to the product's team, or to the CPO Office — dispatch record. 4. CoS — on a package marked ready by the team, send it to the Independent Package Auditor — audit request. 5. CoS — on a passed audit and the owner's decision, freeze the package and send it on the product line — sent package with its manifest hash. 6. CoS — route each engineering request to the product's team; chase answers against the waiting deadline — routing record. 7. CoS — prepare the weekly review brief for the Chief Product Officer — review brief |
| States | `received` → `dispatched` → `in team` → `ready` → `audited` → `decided` → `sent`; `returned`; `held` (on a stop) |
| Failure and recovery | raise, never guess; two failures on the same step stop and go to the Chief Product Officer |
| Records | the Office record and the Work Item record, in `-records` |
| Cadence | continuous; the review brief weekly, on `review_day` |
| Measures | packages refused by the auditor — count per week — no target set; questions open past deadline — count — no target set |
#### Role card
| Field | Content |
|---|---|
| Name | Product Core Chief of Staff |
| Position and seat | `[ORG]CELL-PCCS`; its accountable `[ORG]HOAC-ACS` seat, the Chief Product Officer |
| Performed by | an agent (its bot identity card in `cards/bots/`) |
| Purpose | the door of every input, and the holder of the product line |
| Authority limits | alone: record, route, dispatch, send a passed and decided package, chase; needs the owner: anything that changes a product; never: decide, accept, sign, change a rate, write code |
| Write location | the Office record and the Work Item record |
| Reports to | the Chief Product Officer |
| Escalation | to the product's owner position for a product matter; to the Chief Product Officer otherwise |
| Tools and access | the product line, the Source Lifecycle output socket, the rate store read-back and the signal source, through the Panel; never credentials in instructions |
| Deputy and cover | the Chief Product Officer holds its work |
| Fixed test and score | TEST-PC-PCCS v1 |
| Card version and status | v0.1.0 · draft |
#### Fixed test
TEST-PC v1, case 37 (the default Chief of Staff test, (a) to (h)), and cases 1, 2, 11, 14 to 16, 25 to 27, 39, 41, 44, 45 · result `NOT_RUN`

### 4.3 Input socket
#### Definition
Default · this AIOC's standard format: a Work Item (ID + version) with its sources by reference. Converters: product request; source reference; product signal; engineering request; rate record read-back.
#### Process (SOP)
Default. Each converter checks the shape of its input and refuses with a reason: a product request with no requesting position; a source that does not come from Source Lifecycle's output socket; a signal with no product or no date; an engineering request that cites no package manifest hash; a rate read-back whose hash does not match the record written.
#### Role card
Default; Performed by: the Chief of Staff.
#### Fixed test
TEST-PC v1, case 39 (one good and one bad sample per converter) · result `NOT_RUN`

### 4.4 Panel
#### Definition
Default. The Panel shows, per product, its stage, its team, its open questions from engineering, its open acceptances, its rates and their history, and its explainers; and, for the CPO Office, the portfolio and the review outcomes.
#### Process (SOP)
Default.
#### Role card
Default.
#### Fixed test
TEST-PC v1, case 40 (the default Panel test) · result `NOT_RUN`

---

## 5. Functional capabilities

### 5.0 The stages: input, output, done-test

The work of each product runs in the eight stages of Protocol §18, item 6, in order, carried by the product's one team. The CPO Office's capabilities (5.1, 5.2, 5.10, 5.11) run beside them. A product moves to the next stage only when the stage's done-test passes and its owner position decides the move; a skipped stage fails (TEST-PC v1, case 20).

| ID | Stage | Run state | Gate | Exact input | Exact output | Done-test | Human decision |
|---|---|---|---|---|---|---|---|
| P1 | Research and opportunity | `researching` | G1 | the intake record; sources by reference | the research record (5.3) | every claim labelled `sourced`, `inferred` or `not given`; the opportunity, customer and evidence stated (case 19) | the owner position: go to P2, hold, or stop |
| P2 | The PRD and its feature packages | `specifying` | G2 | the research record; the shared templates | the PRD and feature packages (Annex A.2, A.3) | no blank field ("none" is an answer); every feature has acceptance criteria; passed by the Independent Package Auditor (cases 7, 21, 22) | the owner position: go to P3 |
| P3 | Design | `designing` | G3 | the PRD; the design system | flows, a screen for every state, copy in every language the product serves (Annex A.4) | every state and every language present; deviations from the design system recorded (cases 23, 24) | the owner position: freeze the package and send it (P4) |
| P4 | Partnership in build | `in build` | G4 | the frozen package; engineering requests on the product line | answers, first-look notes, acceptance criterion by criterion | every criterion accepted with its evidence, or the package revised as a new version (cases 25 to 28) | the owner position: accept each criterion |
| P5 | Launch | `launching` | G5 | the accepted build; the launch checks | the launch record | every launch check closed: package accepted, explainers filed, rates set, support ready (case 29) | the owner position: launch |
| P6 | Run | `running` | — (continuous) | product signals; rate requests | rate records; performance and profit-and-loss records; communications; complaint routes | every signal recorded and routed; every rate a versioned record (cases 8, 30 to 32) | the owner position: each rate change |
| P7 | Explainers and supporting documents | with P2 to P6 | G7 | the PRD, the design, the rates | the explainer set, filed into Source Lifecycle (Annex A.5) | every product has its explainers, versioned and filed, revised before a change launches (cases 13, 33) | the owner position: file |
| P8 | Refresh or retire | from a review outcome | G8 | the review outcome | a new P1 to P3 cycle, or the retirement record | a refresh enters P1 as a new version; a retirement closes rates, explainers and the team (case 35) | the Chief Product Officer: retire, under `retire-unit` for the team |

A product goes back from P4 to P2 or P3 only as a new package version, when a question from the engineering AIOC is answered by a change to the product (Protocol §18, item 10).

### 5.1 Product Intake
#### Definition
| Field | Content |
|---|---|
| Name | Product Intake |
| What it is | The CPO Office's intake of product work: product direction from the Requesting Authority and product requests from each company of the organisation, each recorded and routed to one product's team or opened as a product proposal |
| Purpose | Every product matter has one home, and nothing about the how or the when is decided here |
| Scope | does: record, classify (what or why; how or when), route, open a proposal; does not: decide a product, start a build, answer for engineering |
| Inputs | product requests (Work Items, references only) through the HU input port |
| Outputs | an intake record; a dispatch to a team; a proposal to the Chief Product Officer; a returned item to the engineering AIOC for a how or when matter |
| Limits | no raw idea goes to the engineering AIOC; nothing is routed to a person by name |
| Sources | Protocol §18, items 2, 3, 10; card `product-core.part-card.json` v1, inputs 1 |
| Status | draft |
| Done when | the intake record is complete and the item is routed or returned (TEST-PC v1, cases 2, 14, 15) |
#### Process (SOP)
| Field | Content |
|---|---|
| Trigger | a product request at the HU input port |
| Steps | 1. Product Intake Clerk — record the requesting position, the company or market, what is asked and why, its sources by reference — intake record. 2. Product Intake Clerk — classify: what or why (here), how or when (the engineering AIOC) — classification with its reason. 3. Chief of Staff — return a how or when matter to the engineering AIOC — returned item. 4. Portfolio Keeper — find the product in the portfolio; route to its team; or open a product proposal — dispatch, or proposal. 5. Chief Product Officer — decide a proposal: a new product (and its team, 5.2), part of an existing product, or no — decision |
| States | `received` → `classified` → `routed` / `proposed` / `returned` |
| Failure and recovery | a request with no requesting position is refused with its reason; an unclear request goes back to its sender as a question, never guessed |
| Records | the intake record, in `-records` |
| Cadence | continuous |
| Measures | intake records routed within the waiting deadline — share — no target set |
#### Role card
| Field | Content |
|---|---|
| Name | Product Intake Clerk |
| Position and seat | `[ORG]CELL-PIC`, in the CPO Office Pod; its accountable `[ORG]HOAC-ACS` seat, the Chief Product Officer |
| Performed by | an agent |
| Purpose | record and classify every product request |
| Authority limits | alone: record and classify; needs the owner: none; never: decide, route to a person by name, answer for engineering |
| Write location | the intake record |
| Reports to | the Chief of Staff |
| Escalation | to the Chief Product Officer |
| Tools and access | the Work Item queue, through the Panel |
| Deputy and cover | the Chief of Staff |
| Fixed test and score | TEST-PC-PIC v1 |
| Card version and status | v0.1.0 · draft |
#### Fixed test
TEST-PC v1, cases 2, 14, 15 · result `NOT_RUN`

### 5.2 Portfolio and Categories
#### Definition
| Field | Content |
|---|---|
| Name | Portfolio and Categories |
| What it is | The one register of the organisation's products: each product in exactly one category, each category of one of four kinds, each product with one owner position and one team, its stage, and the companies and markets it is configured for |
| Purpose | One product, one owner, one team, one category; no capability recorded as a product; no product copied per company |
| Scope | does: keep the register; check it; propose a new team for a new product; does not: decide which products the organisation has, or what each category holds |
| Inputs | decisions of the Chief Product Officer; stage moves from the teams; the organisation's category record, by reference (slot `categories_record`) |
| Outputs | the portfolio register (Annex C); the proposal for a new team (`create-or-install-unit`, signed by the Chief Product Officer) |
| Limits | the organisation's categories and products never appear in the Library or in this file (Protocol §18, item 4); a capability is never a product, even when it has a fee, a screen or a route |
| Sources | Protocol §18, items 4, 5, 9 |
| Status | draft |
| Done when | every product row is complete and passes the register checks (TEST-PC v1, cases 4, 5, 10, 17, 18) |
#### Process (SOP)
| Field | Content |
|---|---|
| Trigger | a decision of the Chief Product Officer; a stage move; a configuration for a company or market |
| Steps | 1. Portfolio Keeper — write the row: product, category, category kind, owner position, team, stage, configurations — register row. 2. Portfolio Keeper — check: one category; a kind among the four; one owner position holding no other product; not a capability; each company or market a configuration row, never a copy — check record. 3. Portfolio Keeper — on a new product, prepare the new team from the pattern `[ORG]POD-EPT` (§17), with its owner position — team proposal. 4. Chief Product Officer — sign `create-or-install-unit` for the team — signed event in the unit register |
| States | `proposed` → `active` → `retired` |
| Failure and recovery | a failed check holds the row and goes to the Chief Product Officer with its reason |
| Records | the portfolio register, in the writing repository of the instance; the unit register for teams |
| Cadence | on each event; checked in full before each weekly review |
| Measures | rows failing a check — count — target 0 |
#### Role card
| Field | Content |
|---|---|
| Name | Portfolio Keeper |
| Position and seat | `[ORG]CELL-PK`, top Cell of the CPO Office Pod; its accountable seat, the Chief Product Officer |
| Performed by | an agent |
| Purpose | keep the one register of products and their categories |
| Authority limits | alone: write and check rows; needs the owner: a new product, a new team, a change of owner position, a retirement; never: sign, decide a category's content |
| Write location | the portfolio register |
| Reports to | the Chief of Staff |
| Escalation | to the Chief Product Officer |
| Tools and access | the portfolio register and the unit register (read), through the Panel |
| Deputy and cover | the Chief of Staff |
| Fixed test and score | TEST-PC-PK v1 |
| Card version and status | v0.1.0 · draft |
#### Fixed test
TEST-PC v1, cases 4, 5, 10, 17, 18 · result `NOT_RUN`

### 5.3 Research and Opportunity
#### Definition
| Field | Content |
|---|---|
| Name | Research and Opportunity |
| What it is | The first stage of a product: who the customer is, what they need, what the opportunity is, and what the evidence says |
| Purpose | A product starts from evidence, never from an invented figure |
| Scope | does: research from sources by reference and from product signals; state the opportunity; does not: set a price or a target of its own |
| Inputs | the intake record; sources from Source Lifecycle, by reference; product signals |
| Outputs | the research record (Annex A.1) |
| Limits | every claim is labelled `sourced` (with its reference), `inferred` (with its basis) or `not given`; no figure is invented |
| Sources | Protocol §18, item 6.1 |
| Status | draft |
| Done when | gate G1: the research record passes its done-test and the owner position decides (TEST-PC v1, case 19) |
#### Process (SOP)
| Field | Content |
|---|---|
| Trigger | a routed intake record; a refresh outcome (P8) |
| Steps | 1. Product Analyst — gather the sources and signals, by reference — evidence list. 2. Product Manager — write the research record: the customer, the need, the opportunity, the alternatives, the risks, each claim labelled — research record. 3. Product owner — decide: go to P2, hold, or stop — decision |
| States | `researching` → `decided` |
| Failure and recovery | a source not held is asked for through Source Lifecycle; the claim reads `not given` until it is |
| Records | the product's folder, in the writing repository of the instance |
| Cadence | per product |
| Measures | claims `not given` at the decision — count — no target set |
#### Role card
| Field | Content |
|---|---|
| Name | Product Manager (research) and Product Analyst |
| Position and seat | `[ORG]CELL-EPM` and `[ORG]CELL-EPA` in the product's team; its accountable seat, the product's owner position |
| Performed by | agents |
| Purpose | the research record of one product |
| Authority limits | alone: research and write; needs the owner: the stage move; never: invent a figure, decide |
| Write location | the product's folder |
| Reports to | the product's owner position |
| Escalation | to the Chief Product Officer |
| Tools and access | the Source Lifecycle output socket; the signal source, through the Panel |
| Deputy and cover | the team's other agents hold its work |
| Fixed test and score | TEST-PC-EPM v1, TEST-PC-EPA v1 |
| Card version and status | v0.1.0 · draft |
#### Fixed test
TEST-PC v1, cases 19, 20 · result `NOT_RUN`

### 5.4 PRD and Feature Packages
#### Definition
| Field | Content |
|---|---|
| Name | PRD and Feature Packages |
| What it is | The product's requirements document and its feature packages, each feature with acceptance criteria |
| Purpose | Engineering receives only complete product work |
| Scope | does: write the PRD and feature packages from the research record and the shared templates; does not: write code, technical design, an architecture, a schedule or an estimate |
| Inputs | the research record; the document templates (5.11); sources by reference |
| Outputs | the PRD and feature packages (Annex A.2, A.3) |
| Limits | no field is left blank; "none" is an answer; every feature has acceptance criteria; every requirement claim cites its source or is marked **New**; an output that writes code or technical design fails |
| Sources | Protocol §18, item 6.2 |
| Status | draft |
| Done when | gate G2: the Independent Package Auditor passes the PRD and every feature package, and the owner position decides (TEST-PC v1, cases 7, 21, 22) |
#### Process (SOP)
| Field | Content |
|---|---|
| Trigger | the owner's decision at G1 |
| Steps | 1. Product Manager — write the PRD and the feature packages on the shared templates — drafts. 2. Pricing and Economics Analyst — write the product economics section — section draft. 3. Independent Package Auditor — check completeness, acceptance criteria, citations, and that nothing is code or technical design — audit record. 4. Product owner — decide — decision |
| States | `specifying` → `audited` → `decided`; `refused` (back to step 1, with the audit record) |
| Failure and recovery | a refused package goes back with every failing field named; two refusals of the same field go to the owner position |
| Records | the product's folder |
| Cadence | per product version |
| Measures | packages refused at first audit — share — no target set |
#### Role card
| Field | Content |
|---|---|
| Name | Product Manager (PRD) |
| Position and seat | `[ORG]CELL-EPM`; its accountable seat, the product's owner position |
| Performed by | an agent |
| Purpose | the PRD and feature packages of one product |
| Authority limits | alone: write; needs the owner: the stage move; never: write code or technical design, audit its own package |
| Write location | the product's folder |
| Reports to | the product's owner position |
| Escalation | to the Chief Product Officer |
| Tools and access | the document templates; the Source Lifecycle output socket, through the Panel |
| Deputy and cover | the team's other agents hold its work |
| Fixed test and score | TEST-PC-EPM v1 |
| Card version and status | v0.1.0 · draft |

The Independent Package Auditor (`[ORG]CELL-IPA`, in the CPO Office Pod) is bound to an engine of a different family from the writer's where the engine register allows (slot `audit_families_min`); an audit run on the writer's own engine binding stops the package (TEST-PC v1, case 21).
#### Fixed test
TEST-PC v1, cases 7, 21, 22 · result `NOT_RUN`

### 5.5 Design
#### Definition
| Field | Content |
|---|---|
| Name | Design |
| What it is | The product's flows, a screen for every state, its UI and UX, and its copy in every language the product serves |
| Purpose | Engineering builds what is designed, never what it has to guess |
| Scope | does: flows, screens, states, copy, on the shared design system; does not: technical design, components in code |
| Inputs | the decided PRD and feature packages; the design system (5.11); the languages the product serves, from the PRD |
| Outputs | the design part of the package (Annex A.4) |
| Limits | every screen has every state listed in Annex A.4; copy exists in every language the product serves, right to left included where one is served; a deviation from the design system is recorded with its reason |
| Sources | Protocol §18, items 6.3, 8 |
| Status | draft |
| Done when | gate G3: every state and language present and the owner position decides to freeze and send (TEST-PC v1, cases 23, 24) |
#### Process (SOP)
| Field | Content |
|---|---|
| Trigger | the owner's decision at G2 |
| Steps | 1. Product Designer — draw the flows and every screen in every state — design draft. 2. Product Designer — write the copy in every language served — copy set. 3. Independent Package Auditor — check states, languages and design-system use — audit record. 4. Product owner — decide: freeze the package — decision; the Chief of Staff freezes it (Annex A.1) |
| States | `designing` → `audited` → `frozen` |
| Failure and recovery | a missing state or language goes back with its name; a design-system gap goes to the Standards Keeper as a request, never a local fix |
| Records | the product's folder |
| Cadence | per product version |
| Measures | states missing at first audit — count — target 0 |
#### Role card
| Field | Content |
|---|---|
| Name | Product Designer |
| Position and seat | `[ORG]CELL-EPD`; its accountable seat, the product's owner position |
| Performed by | an agent |
| Purpose | the design of one product |
| Authority limits | alone: design and write copy; needs the owner: the freeze; never: technical design, change the design system |
| Write location | the product's folder |
| Reports to | the product's owner position |
| Escalation | to the Chief Product Officer |
| Tools and access | the design system and the design tool, through the Panel |
| Deputy and cover | the team's other agents hold its work |
| Fixed test and score | TEST-PC-EPD v1 |
| Card version and status | v0.1.0 · draft |
#### Fixed test
TEST-PC v1, cases 23, 24 · result `NOT_RUN`

### 5.6 Partnership in Build
#### Definition
| Field | Content |
|---|---|
| Name | Partnership in Build |
| What it is | The team's part while the engineering AIOC builds: it answers questions, takes the first look, and accepts the product criterion by criterion, all on the product line |
| Purpose | The product is built as decided, and every change to it is decided here |
| Scope | does: answer, look, accept; does not: write code or technical design, set the build plan or its dates, speak to a builder or the code host |
| Inputs | engineering requests on the product line, each citing the package manifest hash and the criterion |
| Outputs | answers, first-look notes and acceptances (Work Items) on the product line; a new package version where an answer changes the product |
| Limits | product work reaches the engineering AIOC only as complete packages on the product line; a finding in build that would change the product comes back as a question; acceptance is the owner position's, under live sign-in, one criterion at a time with its evidence |
| Sources | Protocol §18, items 6.4, 10 |
| Status | draft |
| Done when | gate G4: every acceptance criterion of the package accepted with its evidence (TEST-PC v1, cases 11, 25 to 28) |
#### Process (SOP)
| Field | Content |
|---|---|
| Trigger | an engineering request on the product line |
| Steps | 1. Chief of Staff — check that it cites a sent package by manifest hash; route it to the team — routing record. 2. Product Manager — draft the answer from the package; if the answer changes the product, draft a new package version (back to P2 or P3) — answer draft, or version draft. 3. Product owner — decide the answer — decision; the Chief of Staff sends it. 4. Product Manager and Product Designer — on a first-look build, compare it with the package, criterion by criterion — first-look note (never an acceptance). 5. Product owner — on an acceptance request, accept or refuse each criterion with its evidence — acceptance record |
| States | `asked` → `answered`; `first look` → `noted`; `acceptance asked` → `accepted` / `refused` per criterion |
| Failure and recovery | a request that cites no package is returned; an unanswered request past the waiting deadline is raised to the owner position, never closed |
| Records | the Work Item record; the product's folder |
| Cadence | continuous while in build |
| Measures | questions answered within the deadline — share — no target set |
#### Role card
| Field | Content |
|---|---|
| Name | Product owner (acceptance) and Product Manager (answers) |
| Position and seat | `[ORG]CELL-EPO` and `[ORG]CELL-EPM`; the owner position is a HOAC position, accountable to the Chief Product Officer |
| Performed by | the owner position: a person (holders register); the Product Manager: an agent |
| Purpose | answers and acceptance for one product |
| Authority limits | the owner position alone: decide answers, accept criteria; the agent alone: draft; never: accept by an AI, speak to a builder |
| Write location | the Work Item record |
| Reports to | the Chief Product Officer |
| Escalation | to the Chief Product Officer |
| Tools and access | the product line, through the Panel |
| Deputy and cover | an acting owner appointed by the Chief Product Officer |
| Fixed test and score | TEST-PC-EPO v1, TEST-PC-EPM v1 |
| Card version and status | v0.1.0 · draft |
#### Fixed test
TEST-PC v1, cases 11, 25 to 28 · result `NOT_RUN`

### 5.7 Launch
#### Definition
| Field | Content |
|---|---|
| Name | Launch |
| What it is | The decided start of the product, or of a new version, for its companies and markets |
| Purpose | Nothing launches with an open check |
| Scope | does: the launch checks and the launch record; does not: deploy (the engineering AIOC) |
| Inputs | the accepted build; the explainer set; the rate records; support readiness |
| Outputs | the launch record (Annex A.6) |
| Limits | every launch check is closed before the decision: package accepted, explainers filed, rates set, support ready, configuration per company and market set |
| Sources | Protocol §18, item 6.5 |
| Status | draft |
| Done when | gate G5: every check closed and the owner position decides (TEST-PC v1, case 29) |
#### Process (SOP)
| Field | Content |
|---|---|
| Trigger | every criterion accepted at G4 |
| Steps | 1. Product Manager — fill the launch checks, each with its evidence — launch record draft. 2. Product owner — decide the launch — decision. 3. Chief of Staff — send the launch decision to the engineering AIOC on the product line — Work Item |
| States | `launching` → `launched` |
| Failure and recovery | an open check holds the launch; it is never closed by assertion |
| Records | the product's folder |
| Cadence | per launch |
| Measures | launches held for an open check — count — no target set |
#### Role card
| Field | Content |
|---|---|
| Name | Product Manager (launch) |
| Position and seat | `[ORG]CELL-EPM`; its accountable seat, the product's owner position |
| Performed by | an agent |
| Purpose | the launch record of one product |
| Authority limits | alone: fill checks; needs the owner: the launch; never: launch |
| Write location | the product's folder |
| Reports to | the product's owner position |
| Escalation | to the Chief Product Officer |
| Tools and access | through the Panel |
| Deputy and cover | the team's other agents |
| Fixed test and score | TEST-PC-EPM v1 |
| Card version and status | v0.1.0 · draft |
#### Fixed test
TEST-PC v1, case 29 · result `NOT_RUN`

### 5.8 Run
#### Definition
| Field | Content |
|---|---|
| Name | Run |
| What it is | The product's life in use: pricing and every rate that moves over time; performance and the product's profit and loss; customer communications and retention; customer voice and complaints; operations and upkeep |
| Purpose | The team that made the product keeps it, and every rate is data the team changes without a code release |
| Scope | does: rates as versioned data; performance and profit-and-loss records from source records; communications; routing of complaints; upkeep requests; does not: set a money commitment of its own; change code |
| Inputs | product signals; rate requests; sources by reference |
| Outputs | rate records (Annex B); performance and profit-and-loss records; communications; complaint routes; upkeep requests on the product line |
| Limits | every price, fee and rate is a versioned record with an effective date, a reason and the record it replaces; it is changed without a code release; every change can be reversed, by a new record that restores the earlier value; whether a new rate reaches existing deals follows the product's own terms, cited; no figure is invented |
| Sources | Protocol §18, items 6.6, 7 |
| Status | draft |
| Done when | each rate record reads back with its hash; every signal is recorded against its product and routed (TEST-PC v1, cases 8, 30 to 32) |
#### Process (SOP)
| Field | Content |
|---|---|
| Trigger | a product signal; a rate request; the review day |
| Steps | 1. Operations and Customer Voice Agent — record each signal against its product, with its source and date; route a complaint on the organisation's complaints path — signal record, complaint route. 2. Pricing and Economics Analyst — draft a rate change: the new value, its effective date, its reason, the record it replaces, the terms that say whether existing deals take it — rate draft. 3. Product owner — decide the rate change under live sign-in (and `commit-money` where the organisation sets it, slot `rate_signers`) — decision. 4. Chief of Staff — write the rate record to the store and read it back — rate record with its hash. 5. Product Analyst — compute performance and the profit and loss from source records only; a missing input reads `not given` — performance record |
| States | rate: `drafted` → `decided` → `written` → `read back`; `reversed` (by a new record) |
| Failure and recovery | a read-back whose hash differs holds the rate and goes to the owner position; a rate changed by a code release is raised as a failure (case 8) |
| Records | the rate and configuration store; the product's folder |
| Cadence | continuous; performance weekly, before the review |
| Measures | rates reversed — count per period — no target set; complaints acknowledged within the organisation's deadline — share — no target set |
#### Role card
| Field | Content |
|---|---|
| Name | Pricing and Economics Analyst; Operations and Customer Voice Agent |
| Position and seat | `[ORG]CELL-EPEA`, `[ORG]CELL-EOCVA`; their accountable seat, the product's owner position |
| Performed by | agents |
| Purpose | rates as data, and the voice of the product's customers |
| Authority limits | alone: draft, record, route; needs the owner: every rate change; never: write a rate without the owner's decision, answer a complaint with a promise no position has made |
| Write location | the product's folder; the rate store only through the Chief of Staff |
| Reports to | the product's owner position |
| Escalation | to the Chief Product Officer |
| Tools and access | the rate store (read), the signal source, through the Panel |
| Deputy and cover | the team's other agents |
| Fixed test and score | TEST-PC-EPEA v1, TEST-PC-EOCVA v1 |
| Card version and status | v0.1.0 · draft |
#### Fixed test
TEST-PC v1, cases 8, 30 to 32 · result `NOT_RUN`

### 5.9 Explainers and Supporting Documents
#### Definition
| Field | Content |
|---|---|
| Name | Explainers and Supporting Documents |
| What it is | The product's explainer and its questions and answers, help articles and user guides, partner materials and internal training, written with the product and filed into Source Lifecycle as sources |
| Purpose | Every product can be explained from one valid version of each document |
| Scope | does: write, version and file; does not: publish outside the organisation on its own (the organisation's publication path) |
| Inputs | the PRD, the design, the rates, the launch record |
| Outputs | the explainer set (Annex A.5), filed into Source Lifecycle |
| Limits | a product with no explainers fails; a change that launches revises its explainers first; customer-facing text goes through the organisation's own review of public text before it is seen outside |
| Sources | Protocol §18, item 6.7; Protocol §13 |
| Status | draft |
| Done when | gate G7: every document of the set is versioned and filed, and reads back from Source Lifecycle (TEST-PC v1, cases 13, 33) |
#### Process (SOP)
| Field | Content |
|---|---|
| Trigger | the owner's decision at G2; every change to the product |
| Steps | 1. Documentation Writer — write each document of the set on the shared templates — drafts. 2. Product owner — approve each for filing — decision. 3. Chief of Staff — file each into Source Lifecycle, the owner position as the contributor — filing receipt |
| States | `drafting` → `approved` → `filed` |
| Failure and recovery | a filing refused by Source Lifecycle goes back with its reason |
| Records | Source Lifecycle; the product's folder (by reference) |
| Cadence | per product version |
| Measures | products with a missing document — count — target 0 |
#### Role card
| Field | Content |
|---|---|
| Name | Documentation Writer |
| Position and seat | `[ORG]CELL-EDW`; its accountable seat, the product's owner position |
| Performed by | an agent |
| Purpose | the explainer set of one product |
| Authority limits | alone: write; needs the owner: filing; never: publish outside the organisation |
| Write location | the product's folder; Source Lifecycle only through the Chief of Staff |
| Reports to | the product's owner position |
| Escalation | to the Chief Product Officer |
| Tools and access | the document templates; Source Lifecycle's intake, through the Panel |
| Deputy and cover | the team's other agents |
| Fixed test and score | TEST-PC-EDW v1 |
| Card version and status | v0.1.0 · draft |
#### Fixed test
TEST-PC v1, cases 13, 33 · result `NOT_RUN`

### 5.10 Product Review, Refresh or Retire
#### Definition
| Field | Content |
|---|---|
| Name | Product Review, Refresh or Retire |
| What it is | The CPO Office's weekly product review, with an outcome for each product (keep, fix, grow or retire), and the refresh or retirement that follows |
| Purpose | Every product is looked at every week, from its evidence |
| Scope | does: the review brief, the outcomes, the refresh or retirement; does not: decide for a product owner what the product's content is |
| Inputs | each product's stage, performance record, signals, open questions and rates |
| Outputs | the review record; product review outcomes; a refresh (back to P1) or a retirement record (Annex A.7) |
| Limits | an outcome cites its evidence; a retirement closes the product's rates, withdraws its explainers in Source Lifecycle, sends its customer communications, and retires its team under `retire-unit` |
| Sources | Protocol §18, items 3, 6.8; card outputs 5 |
| Status | draft |
| Done when | gate G8: every product has an outcome at the review; a retirement record has every closing step done (TEST-PC v1, cases 34, 35) |
#### Process (SOP)
| Field | Content |
|---|---|
| Trigger | `review_day` |
| Steps | 1. Product Review Secretary — prepare the brief, one row per product, from its records — review brief. 2. Chief Product Officer, with each owner position — decide each outcome — review record. 3. Chief of Staff — send each outcome to the Requesting Authority's Cell — Work Item. 4. On a retirement: the team closes rates, withdraws explainers, sends communications; the Chief Product Officer signs `retire-unit` for the team — retirement record |
| States | `briefed` → `reviewed`; retirement: `deciding` → `closing` → `retired` |
| Failure and recovery | a product with no outcome for two reviews is raised to the Chief Product Officer |
| Records | the review record, in `-records` |
| Cadence | weekly |
| Measures | products with no outcome — count — target 0 |
#### Role card
| Field | Content |
|---|---|
| Name | Product Review Secretary |
| Position and seat | `[ORG]CELL-PRS`, in the CPO Office Pod; its accountable seat, the Chief Product Officer |
| Performed by | an agent |
| Purpose | the weekly review brief and record |
| Authority limits | alone: prepare and record; needs the owner: every outcome; never: decide an outcome |
| Write location | the review record |
| Reports to | the Chief of Staff |
| Escalation | to the Chief Product Officer |
| Tools and access | the portfolio register and each product's records (read), through the Panel |
| Deputy and cover | the Chief of Staff |
| Fixed test and score | TEST-PC-PRS v1 |
| Card version and status | v0.1.0 · draft |
#### Fixed test
TEST-PC v1, cases 34, 35 · result `NOT_RUN`

### 5.11 Shared Standards
#### Definition
| Field | Content |
|---|---|
| Name | Shared Standards |
| What it is | The standards the CPO Office keeps once, for every team: the design system, the pricing models, the measurement tools and the document templates |
| Purpose | Shared standards, not shared work |
| Scope | does: keep, version and improve the standards on the teams' requests; does not: any product's own work |
| Inputs | requests from the teams; decisions of the Chief Product Officer |
| Outputs | versioned standards; notices of each new version to every team |
| Limits | a standard does no product's own work (Protocol §18, item 8); every team uses the current version, or records why not |
| Sources | Protocol §18, item 8 |
| Status | draft |
| Done when | each new version is decided, versioned and noticed to every team (TEST-PC v1, cases 9, 24, 36) |
#### Process (SOP)
| Field | Content |
|---|---|
| Trigger | a request from a team; a review finding |
| Steps | 1. Standards Keeper — draft the change to the standard — draft. 2. Chief Product Officer — decide — decision. 3. Standards Keeper — publish the new version to every team — notice |
| States | `requested` → `drafted` → `decided` → `published` |
| Failure and recovery | a request that is a product's own work goes back to its team |
| Records | the standards, in the writing repository of the instance |
| Cadence | on request |
| Measures | teams on an old version — count — no target set |
#### Role card
| Field | Content |
|---|---|
| Name | Standards Keeper |
| Position and seat | `[ORG]CELL-SK`, in the CPO Office Pod; its accountable seat, the Chief Product Officer |
| Performed by | an agent |
| Purpose | the shared standards of the part |
| Authority limits | alone: draft and publish a decided version; needs the owner: every change; never: do a product's own work |
| Write location | the standards |
| Reports to | the Chief of Staff |
| Escalation | to the Chief Product Officer |
| Tools and access | through the Panel |
| Deputy and cover | the Chief of Staff |
| Fixed test and score | TEST-PC-SK v1 |
| Card version and status | v0.1.0 · draft |
#### Fixed test
TEST-PC v1, cases 9, 24, 36 · result `NOT_RUN`

---

## 6. Coordination and routes

- **Whom it works with.** The engineering AIOC, on the product line only; Source Lifecycle, through its output socket and its intake; the Requesting Authority's Cell and each company's positions, through the HU ports; the organisation's signal sources and its rate and configuration store, through the tool gateway. Always through the 49GAION Operating Protocol: one Work Item per hand-off, this AIOC's Chief of Staff as its door.
- **Routing rows this AIOC contributes.** A product request → `[ORG]AIOC-PC`. A how or when matter found here → the engineering AIOC. A product finding found in build → back to `[ORG]AIOC-PC` as a question. A product document → `[ORG]AIOC-SL` as a source.
- **Requests and objections.** Owners do not design or change this AIOC's AIs: every proposal, correction or critique is a `design-proposal` Work Item to OCO; where they disagree, the Chief Product Officer may hold the objection open until it reaches the HOAC seat accountable for OCO, which decides.

## 7. Records and where things live

| Record | Home | Source rule |
|---|---|---|
| This blueprint, its decisions, its tests and its cards | the instance's writing repository `<org>aioc-pc`; the mother in `github.com/49g-holding/49GAION-product-core` | one home for each thing |
| The portfolio register, the categories, each product's folder (research, PRD, design, run records, decisions), the shared standards | the instance's writing repository `<org>aioc-pc`, private | one home; never in the Library |
| Rates and configuration | the rate and configuration store (versioned) | the store is the one home; the product's folder cites it |
| Explainers and supporting documents | Source Lifecycle, as sources | one valid version each (Protocol §13) |
| Run records (intake, Office, review) | `<org>aioc-pc-records`; personal data only in `-records-restricted` | Naming Standard R9 |
| Work Items | the shared queue | Protocol §2 |
| Code that runs | the engineering AIOC's code project; never here | Protocol §18, item 10 |

## 8. Tools and the shared AI gateway

| Tool | Existing shared tool, or new | If new: asked of the builder as |
|---|---|---|
| The product line | new: a typed port between this AIOC and the engineering AIOC, at the tool gateway | a port under `connect-external-port`, with the package contract (Annex A; `upstream/PROPOSALS.md`, item 1) |
| Rate and configuration store | new or existing, per organisation: versioned records, effective dates, read-back, reversal | a store that keeps every version and its reason |
| Design tool | existing, per organisation | a connector, recorded by role |
| Source Lifecycle | existing Library part | its output socket and its intake |

All model calls go through the tool gateway of the `[ORG]AION`. Each tool is reached through a swappable connector, recorded by role; access is granted and withdrawn in the Panel. This AIOC's AI usage is metered separately; its budget cap is set in §15.

| Tool role | Connector | Access managed in | Part card version |
|---|---|---|---|
| the product line to the engineering AIOC | `<engineering AIOC> product line port` | Panel | v1 |
| source of record (the output socket of Source Lifecycle) | `[ORG]AIOC-SL output socket` | Panel | v1 |
| rate and configuration store (versioned) | `<store>` | Panel | v1 |
| tool gateway (signatures, metering, the stop door) | the `[ORG]AION`'s gateway | Panel | v1 |

**Mechanism register.** A row is never deleted.

| ID | Mechanism | What it does | Where it lives | Today | Target |
|---|---|---|---|---|---|
| M-01 | Portfolio register | one row per product: category, kind, owner position, team, stage, configurations | instance writing repository | decided, not built | build |
| M-02 | Package freeze | content-addresses a package: manifest and parts by hash | the Chief of Staff's code step | decided, not built | build |
| M-03 | Package audit | completeness, criteria, citations, no code | the Independent Package Auditor | decided, not built | build |
| M-04 | Rate records | versioned rates with effective date, reason, replaces; read-back; reversal | the rate and configuration store | decided, not built | build |
| M-05 | Signal record | every signal against its product, with source and date | `-records` | decided, not built | build |
| M-06 | Weekly review | the brief and the outcomes | `-records` | decided, not built | build |

**Reserve.**

| ID | Idea | Why held | Reconsider when |
|---|---|---|---|
| R-01 | A Library contract for the product package | no second part reads it yet; Annex A gives the field lists | the engineering AIOC's mother asks for it (`upstream/PROPOSALS.md`, item 1) |
| R-02 | An origin kind in Source Lifecycle for product documents | the documents enter as ordinary sources from the owner position | Source Lifecycle needs to tell them apart (`upstream/PROPOSALS.md`, item 2) |

## 9. Fixed tests: index, triggers and scores

| Capability | Test ID and version | Evidence level | Last run | Result |
|---|---|---|---|---|
| Office | TEST-PC v1, case 38 | MEASURED | — | `NOT_RUN` |
| Chief of Staff | TEST-PC v1, case 37 | MEASURED | — | `NOT_RUN` |
| Input socket | TEST-PC v1, case 39 | MEASURED | — | `NOT_RUN` |
| Panel | TEST-PC v1, case 40 | MEASURED | — | `NOT_RUN` |
| Product Intake | TEST-PC v1, cases 2, 14, 15 | MEASURED | — | `NOT_RUN` |
| Portfolio and Categories | TEST-PC v1, cases 4, 5, 10, 17, 18 | MEASURED | — | `NOT_RUN` |
| Research and Opportunity | TEST-PC v1, cases 19, 20 | MEASURED | — | `NOT_RUN` |
| PRD and Feature Packages | TEST-PC v1, cases 7, 21, 22 | MEASURED | — | `NOT_RUN` |
| Design | TEST-PC v1, cases 23, 24 | MEASURED | — | `NOT_RUN` |
| Partnership in Build | TEST-PC v1, cases 11, 25 to 28 | MEASURED | — | `NOT_RUN` |
| Launch | TEST-PC v1, case 29 | MEASURED | — | `NOT_RUN` |
| Run | TEST-PC v1, cases 8, 30 to 32 | MEASURED | — | `NOT_RUN` |
| Explainers and Supporting Documents | TEST-PC v1, cases 13, 33 | MEASURED | — | `NOT_RUN` |
| Product Review, Refresh or Retire | TEST-PC v1, cases 34, 35 | MEASURED | — | `NOT_RUN` |
| Shared Standards | TEST-PC v1, cases 9, 24, 36 | MEASURED | — | `NOT_RUN` |
| The whole AIOC | TEST-PC v1, cases 1 to 48 (`tests/TEST-PC.md`) | MEASURED | — | `NOT_RUN` |

- **Re-run triggers:** any change to a model, instructions, this AIOC's card, this blueprint, Protocol §18, a shared standard, a tool or its access, or the product line's contract.
- **The Library's cases.** TEST-PC v1 keeps the Library's TEST-PRODUCT-CORE v1, cases 1 to 13, unchanged, as its own cases 1 to 13 (`tests/TEST-PC.md`). No case is weakened.
- **Complete** only when every capability's test has a visible result. `NOT_RUN` is never PASS.

**Checks that are not fixed tests.**

| Check | Placement | Budget per item | Degradation order | Blocks only for |
|---|---|---|---|---|
| Package completeness (the Independent Package Auditor) | on the verdict record, before the owner's decision | one audit per package version | none: it always runs | a blank field, a feature with no criteria, code or technical design |
| Rate read-back | after completion of the write | one read per record | none | a hash that differs |

- **Discriminating evidence.** A passing check counts only if it has been shown able to fail on the case it guards; evidence is written by the runner, never by the worker.

## 10. Build: what is generated from this file

| Built thing | Generated from | Recorded where |
|---|---|---|
| Panel profile | §0, §1, §3, §4.4, §5 role cards | the panel profile names this file's commit |
| Back office | §4.2 role card and SOP; §4–§5 definitions and SOPs | the back office records the commit it was built from |
| Card in the protocol AIOC's map | §1 | the protocol AIOC's register links this file |
| Unit cards and bot identity cards | §17 card data | `cards/`, by `tools/make_cards.py` |
| Panel Health section | §9 results; stuck, returned and late Work Items | the Panel |

**Delivery path:** definition change → tests → Panel and Back office update → one-click rollback to the previous commit.

## 11. Exceptions

- **Office.** A single Chief of Staff; an Office only when proposed and approved (§4.1).
- **Product teams are made from a pattern.** §17 sets one product team, named `Example`, as the pattern. An instance makes one team per product from it, named by the product, each a Pod created under `create-or-install-unit` and checked against its register before first use (Naming Standard §5, R15). The pattern itself is never created as a team.
- **No code project.** Product Core writes no code (Protocol §18, item 6.4).

## 12. Lessons and proposals to the mother

One dated line per lesson, each written without an organisation's details. Nothing is proposed upstream without the word of the governing seat of 49GAION; the drafts are in `upstream/PROPOSALS.md`.

1. 2026-10-16 · The product line has no Library contract; every organisation would invent its own package shape. Annex A gives the field lists; a contract is drafted (`upstream/PROPOSALS.md`, item 1). Test case 25 checks the freeze.

## 13. For the `[ORG]HOAC-ACS` seat, and every decision only a human seat can take

| ID | Decision | Who decides | Until decided |
|---|---|---|---|
| H-01 | Who occupies the Chief Product Officer position and each owner position, and how | top management's own mechanism; this AIOC never sees it (Standard §1.1, item 9) | acts that need the position's signature wait |
| H-02 | The organisation's products and categories (its own record, slot `categories_record`) | the Chief Product Officer, under the Requesting Authority's direction | no product team is created |
| H-03 | **Money.** Whether a rate change is also a money commitment (`commit-money`), its limits per product, and who signs it (slot `rate_signers`) | the Cell carrying `[ORG]HOAC-TM`, with the Requesting Authority | every rate change is signed by the owner position only, and none above the limits the organisation has set elsewhere is written |
| H-04 | **Legal.** Each product's terms, including whether a new rate reaches existing deals; review of customer-facing explainers before they are seen outside | the position the organisation names for legal review | no launch with open terms (case 29) |
| H-05 | **People.** The owner position of each new product (`create-or-install-unit`, `change-filler`) | the Chief Product Officer | the product has no team |
| H-06 | The engineering AIOC's code and the product line's grant (`connect-external-port`) | the Cell carrying `[ORG]HOAC-TM` | no package is sent |
| H-07 | Approve this blueprint `v0.1.0`, with the exceptions of §11, as the design of `[ORG]AIOC-PC` | the human hub | it stays a draft; nothing is installed |
| H-08 | The complaints path of the organisation, which the Run capability routes into | the position the organisation names | complaints are recorded and held |

## 14. Change log

| Blueprint version | Date | Change | Template version | Commit |
|---|---|---|---|---|
| v0.1.0 | 2026-10-16 | First blueprint of `[ORG]AIOC-PC`, the mother blueprint of 49GAION Product Core, from the Protocol section Product Core (§18) and the part card v1; TEST-PC v1 (48 cases, `NOT_RUN`), keeping TEST-PRODUCT-CORE v1 cases 1 to 13 unchanged; the CPO Office and the product team pattern; the field lists of the package, the rate record and the portfolio register (`decisions/DR-0001`; `49GAION/DR-0024`) | v1.5.0 at `1abae80` | this repository, pull request #1 |

---

## 15. Configuration

Every slot is filled by the organisation; an AIOC with any empty slot does not pass the joining test (Protocol §11). Each value records who set it, when, and in which version.

| Slot | Value | Default offered by 49GAION | Set by | Date | Version | Replaces |
|---|---|---|---|---|---|---|
| HOAC seat accountable for OCO | | none: must be set | | | | |
| OCO of this `[ORG]AION` | `<code of [ORG]AIOC-OCO>` | none: must be set | | | | |
| Discussion limits | | none: must be set | | | | |
| Waiting deadlines (per status) | | none: must be set | | | | |
| Bounce limit | | none: must be set | | | | |
| Chain depth | | none: must be set | | | | |
| Halt-request priority | | immediate | | | | |
| Budget cap | | none: must be set | | | | |
| Unattended action | | read-record-triage | | | | |
| Final authority | the `[ORG]HOAC-GOV` position | none: must be set | | | | |
| **The Requesting Authority** (`requesting_authority_cell`) | | none: must be set | | | | |
| **The engineering AIOC** (`engineering_aioc`) | | none: must be set | | | | |
| **The category record** (`categories_record`), by reference | | none: must be set | | | | |
| **Review day** (`review_day`) | | none: must be set | | | | |
| **Rate signers** (`rate_signers`), per product, and whether a rate change is also `commit-money` | | the owner position; `commit-money` not set | | | | |
| **Audit engine families** (`audit_families_min`) | | 2 | | | | |
| Sensitivity classes of this AIOC's work and the default filler kind of each | | none: must be set | | | | |
| Delegation ladder of each Chief of Staff | | only prepares, for every class | | | | |
| Stuck-item thresholds per status | | none: must be set | | | | |
| Loop breaker | | 3 runs in 2 hours | | | | |

---

## 16. Type

- **Type:** Structural, as in §0.
- **Why this AIOC exists in this organisation:** `<organisation>` has one product division, shared by every company it runs, so that every product has one home for its what and its why.
- **Type-specific test:** TEST-PC v1, cases 1 to 13 · result `NOT_RUN`.

## 17. Cells and Pods

The parts inside this AIOC (`docs/CELLS-AND-PODS.md` of `49GAION-aioc`). The role and nature of this AIOC are read from the type of its top Cell, the Chief Product Officer. Every field that points to a human takes a position code only.

| Code | Kind | Type | Filler kind | HOAC label | Parent | Fixed test (owner) | External ports |
|---|---|---|---|---|---|---|---|
| `[ORG]CELL-CPO` | CELL | Human Seat | human | `[ORG]HOAC-ACS` | `[ORG]AIOC-PC` | TEST-PC-CPO v1 (the Cell carrying `[ORG]HOAC-TM`) | none |
| `[ORG]CELL-PCCS` | CELL | AI Chief of Staff | ai | none | `[ORG]AIOC-PC` | TEST-PC-PCCS v1 (`[ORG]CELL-CPO`) | `eng-out`, `eng-in`, `sl-in`, `sl-out`, `rates-out`, `rates-in`, `signals-in` |
| `[ORG]POD-PCCO` | POD | AI Pod | — | none | `[ORG]AIOC-PC` | TEST-PC-PCCO v1 (`[ORG]CELL-CPO`) | — |
| `[ORG]CELL-PIC`, `-PK`, `-SK`, `-PRS`, `-IPA` | CELL | AI Agent | ai | none | `[ORG]POD-PCCO` | TEST-PC-PIC v1 … TEST-PC-IPA v1 (`[ORG]CELL-CPO`) | none |
| `[ORG]POD-EPT` (pattern) | POD | Product Team | — | `[ORG]HOAC-ACS` | `[ORG]AIOC-PC` | TEST-PC-EPT v1 (`[ORG]CELL-CPO`) | — |
| `[ORG]CELL-EPO` (pattern) | CELL | Human Seat | human | `[ORG]HOAC-ACS` | `[ORG]POD-EPT` | TEST-PC-EPO v1 (`[ORG]CELL-CPO`) | none |
| `[ORG]CELL-EPM`, `-EPD`, `-EPA`, `-EPEA`, `-EOCVA`, `-EDW` (pattern) | CELL | AI Agent | ai | none | `[ORG]POD-EPT` | TEST-PC-EPM v1 … TEST-PC-EDW v1 (`[ORG]CELL-EPO`) | none |

**The product team pattern** (Protocol §18, item 5). `[ORG]POD-EPT` and its Cells are the pattern for one product's team, named here for a product called `Example`. An instance makes one Pod per product from it: the product's name replaces `Example` in every full name, and every code is the initials of its full name (Naming Standard R15), checked against the organisation's register before first use (§5). One owner position, human, with its HOAC label; six AI members by function: product management and the PRD, design, analysis, pricing and product economics, operations and customer voice, documentation. The team stays with its product for every stage.

**The card data (the blueprint governs).** `tools/make_cards.py` expands the block below into the complete unit cards and bot identity cards, writes them into `cards/`, and checks them against the schemas of `49GAION-protocol`, Naming Standard R15, and this blueprint.

```yaml
parts:
  defaults:
    accountable_to: "[ORG]CELL-CPO"
    card_version: "v0.1.0"
    version: "0.1.0"
    lifecycle_state: "designed"
    test_version: "v1"
    test_owner: "[ORG]CELL-CPO"
    accountable_human: "[ORG]HOAC-ACS (the Chief Product Officer, [ORG]CELL-CPO)"
    audit_trail: "the run record of [ORG]AIOC-PC"
    hu_in: ["run control and configuration from the Chief Product Officer (never a source)"]
    hu_out: ["report to the Chief Product Officer"]
  cells:
    - code: "[ORG]CELL-CPO"
      full_name: "Chief Product Officer"
      parent: "[ORG]AIOC-PC"
      type: "Human Seat"
      filler_kind: "human"
      hoac: "[ORG]HOAC-ACS"
      accountable_to: "[ORG]CELL-TMS"       # example code of the Cell carrying [ORG]HOAC-TM
      entity: "<entity>"
      authority_scope:
        decision_types: ["create-or-install-unit", "retire-unit", "change-filler", "appoint-acting-filler", "delegate-authority", "change-fixed-test-or-threshold", "restart-stopped-unit"]
        entity: "<entity>"
        expires: "2027-10-15"                # placeholder; each organisation sets it
        authority: "delegated"
      test: { id: "TEST-PC-CPO", cases: "3, 18, 34, 35, 42, 43", owner: "[ORG]CELL-TMS" }
      ai_in: ["review brief", "product proposals", "decision rows"]
      ai_out: ["run control and configuration"]
      hu_in: ["direction from the Cell carrying [ORG]HOAC-TM", "product direction from the Requesting Authority's Cell"]
      hu_out: ["decisions under live sign-in", "report to the Cell carrying [ORG]HOAC-TM"]
    - code: "[ORG]CELL-PCCS"
      full_name: "Product Core Chief of Staff"
      role: "Chief of Staff"
      parent: "[ORG]AIOC-PC"
      type: "AI Chief of Staff"
      filler_kind: "ai"
      cell_kind: "chief-of-staff-cell"
      test: { id: "TEST-PC-PCCS", cases: "1, 2, 11, 14-16, 25-27, 37, 39, 41, 44, 45" }
      ai_in: ["source reference", "product signal", "engineering request", "rate record read-back", "drafts and records of the Pods"]
      ai_out: ["dispatch to a Pod", "audit request", "product package", "answer or acceptance", "rate record", "explainer filing", "product review outcome"]
      hu_in: ["product request (references only)", "a decision of the Chief Product Officer or of an owner position", "run control from the Chief Product Officer"]
      hu_out: ["review brief to the Chief Product Officer", "decision rows to the owner positions", "product review outcome to the Requesting Authority's Cell"]
      external_ports:
        - { port: "eng-out", direction: "output", accepted_content: ["product package", "answer or acceptance", "launch decision"], authority_limit: "the product line only, under the scope signed under connect-external-port over the engineering AIOC; frozen, audited and decided packages only", audit_trail: "unit register; the Work Item record" }
        - { port: "eng-in", direction: "input", accepted_content: ["question", "first-look build", "acceptance request"], authority_limit: "requests that cite a sent package by manifest hash, on the product line only", audit_trail: "unit register; the Work Item record" }
        - { port: "sl-in", direction: "input", accepted_content: ["source reference"], authority_limit: "the read scope signed under connect-external-port over [ORG]AIOC-SL", audit_trail: "unit register; serve log of [ORG]AIOC-SL" }
        - { port: "sl-out", direction: "output", accepted_content: ["explainer filing", "needs request"], authority_limit: "this AIOC's own documents, with the owner position as contributor", audit_trail: "unit register; serve log of [ORG]AIOC-SL" }
        - { port: "rates-out", direction: "output", accepted_content: ["rate record"], authority_limit: "a rate record decided by the product's owner position under live sign-in", audit_trail: "unit register; the store's version log" }
        - { port: "rates-in", direction: "input", accepted_content: ["rate record read-back"], authority_limit: "read only", audit_trail: "unit register; the store's version log" }
        - { port: "signals-in", direction: "input", accepted_content: ["product signal"], authority_limit: "read only, within the scope signed for the signal source", audit_trail: "unit register" }
      bot:
        allowed_actions: ["record and route every input", "dispatch Cells of this AIOC", "send a package for audit", "freeze a decided package and send it on the product line", "route engineering requests and chase answers", "write a decided rate record and read it back", "file an approved document into Source Lifecycle", "prepare the review brief"]
        ask_first_actions: ["a budget above the cap", "any change to configuration", "anything outside its role card"]
    - { code: "[ORG]CELL-PIC", full_name: "Product Intake Clerk", role: "Product Intake Clerk", parent: "[ORG]POD-PCCO", type: "AI Agent", filler_kind: "ai", test: { id: "TEST-PC-PIC", cases: "2, 14, 15" }, ai_in: ["product request"], ai_out: ["intake record", "classification"], bot: { allowed_actions: ["record and classify product requests"], ask_first_actions: ["anything outside its role card"] } }
    - { code: "[ORG]CELL-PK", full_name: "Portfolio Keeper", role: "Portfolio Keeper", parent: "[ORG]POD-PCCO", type: "AI Agent", filler_kind: "ai", test: { id: "TEST-PC-PK", cases: "4, 5, 10, 17, 18" }, ai_in: ["decisions of the Chief Product Officer", "stage moves"], ai_out: ["register row", "check record", "team proposal"], bot: { allowed_actions: ["write and check portfolio rows", "prepare a team proposal from the pattern"], ask_first_actions: ["anything outside its role card"] } }
    - { code: "[ORG]CELL-SK", full_name: "Standards Keeper", role: "Standards Keeper", parent: "[ORG]POD-PCCO", type: "AI Agent", filler_kind: "ai", test: { id: "TEST-PC-SK", cases: "9, 24, 36" }, ai_in: ["requests from the teams"], ai_out: ["standard draft", "version notice"], bot: { allowed_actions: ["draft changes to the shared standards", "publish a decided version"], ask_first_actions: ["anything outside its role card"] } }
    - { code: "[ORG]CELL-PRS", full_name: "Product Review Secretary", role: "Product Review Secretary", parent: "[ORG]POD-PCCO", type: "AI Agent", filler_kind: "ai", test: { id: "TEST-PC-PRS", cases: "32, 34, 35" }, ai_in: ["product records"], ai_out: ["review brief", "review record"], bot: { allowed_actions: ["prepare the weekly review brief", "record the outcomes decided"], ask_first_actions: ["anything outside its role card"] } }
    - { code: "[ORG]CELL-IPA", full_name: "Independent Package Auditor", role: "Independent Package Auditor", parent: "[ORG]POD-PCCO", type: "AI Agent", filler_kind: "ai", test: { id: "TEST-PC-IPA", cases: "7, 21-23, 25" }, ai_in: ["audit request"], ai_out: ["audit record"], bot: { allowed_actions: ["check a package for completeness, criteria, citations, states, languages and the absence of code"], ask_first_actions: ["anything outside its role card"] } }
    - code: "[ORG]CELL-EPO"
      full_name: "Example Product Owner"
      parent: "[ORG]POD-EPT"
      type: "Human Seat"
      filler_kind: "human"
      hoac: "[ORG]HOAC-ACS"
      accountable_to: "[ORG]CELL-CPO"
      entity: "<entity>"
      authority_scope:
        decision_types: []                   # the product's own decisions are ordinary decisions under live sign-in; commit-money is added only where the organisation sets it (§13, H-03)
        entity: "<entity>"
        expires: "2027-10-15"                # placeholder; each organisation sets it
        authority: "delegated"
      test: { id: "TEST-PC-EPO", cases: "5, 20, 28-30, 48", owner: "[ORG]CELL-CPO" }
      ai_in: ["decision rows of its product"]
      ai_out: ["decisions of its product"]
      hu_in: ["direction from the Chief Product Officer"]
      hu_out: ["decisions, acceptances and rate decisions under live sign-in", "report to the Chief Product Officer"]
    - { code: "[ORG]CELL-EPM", full_name: "Example Product Manager", role: "Product Manager", parent: "[ORG]POD-EPT", type: "AI Agent", filler_kind: "ai", accountable_to: "[ORG]CELL-EPO", accountable_human: "[ORG]HOAC-ACS (the product's owner position, [ORG]CELL-EPO)", test: { id: "TEST-PC-EPM", cases: "7, 19, 20, 22, 26, 29", owner: "[ORG]CELL-EPO" }, ai_in: ["intake record", "research evidence", "engineering request"], ai_out: ["research record", "PRD and feature packages", "answer draft", "launch record draft"], bot: { allowed_actions: ["write the research record, the PRD and feature packages", "draft answers and launch records"], ask_first_actions: ["anything outside its role card"] } }
    - { code: "[ORG]CELL-EPD", full_name: "Example Product Designer", role: "Product Designer", parent: "[ORG]POD-EPT", type: "AI Agent", filler_kind: "ai", accountable_to: "[ORG]CELL-EPO", accountable_human: "[ORG]HOAC-ACS (the product's owner position, [ORG]CELL-EPO)", test: { id: "TEST-PC-EPD", cases: "23, 24, 27", owner: "[ORG]CELL-EPO" }, ai_in: ["decided PRD", "design system"], ai_out: ["flows, screens and copy", "first-look note"], bot: { allowed_actions: ["design flows and screens in every state", "write copy in every language served"], ask_first_actions: ["anything outside its role card"] } }
    - { code: "[ORG]CELL-EPA", full_name: "Example Product Analyst", role: "Product Analyst", parent: "[ORG]POD-EPT", type: "AI Agent", filler_kind: "ai", accountable_to: "[ORG]CELL-EPO", accountable_human: "[ORG]HOAC-ACS (the product's owner position, [ORG]CELL-EPO)", test: { id: "TEST-PC-EPA", cases: "19, 32", owner: "[ORG]CELL-EPO" }, ai_in: ["source references", "product signals"], ai_out: ["evidence list", "performance record"], bot: { allowed_actions: ["gather evidence by reference", "compute performance and profit and loss from source records"], ask_first_actions: ["anything outside its role card"] } }
    - { code: "[ORG]CELL-EPEA", full_name: "Example Pricing and Economics Analyst", role: "Pricing and Economics Analyst", parent: "[ORG]POD-EPT", type: "AI Agent", filler_kind: "ai", accountable_to: "[ORG]CELL-EPO", accountable_human: "[ORG]HOAC-ACS (the product's owner position, [ORG]CELL-EPO)", test: { id: "TEST-PC-EPEA", cases: "8, 30", owner: "[ORG]CELL-EPO" }, ai_in: ["rate request", "pricing models", "terms"], ai_out: ["rate draft", "product economics section"], bot: { allowed_actions: ["draft rate changes as versioned records", "write the product economics section"], ask_first_actions: ["anything outside its role card"] } }
    - { code: "[ORG]CELL-EOCVA", full_name: "Example Operations and Customer Voice Agent", role: "Operations and Customer Voice Agent", parent: "[ORG]POD-EPT", type: "AI Agent", filler_kind: "ai", accountable_to: "[ORG]CELL-EPO", accountable_human: "[ORG]HOAC-ACS (the product's owner position, [ORG]CELL-EPO)", test: { id: "TEST-PC-EOCVA", cases: "31", owner: "[ORG]CELL-EPO" }, ai_in: ["product signal"], ai_out: ["signal record", "complaint route", "upkeep request draft"], bot: { allowed_actions: ["record customer voice, complaints, support and performance readings against the product", "route complaints on the organisation's complaints path"], ask_first_actions: ["anything outside its role card"] } }
    - { code: "[ORG]CELL-EDW", full_name: "Example Documentation Writer", role: "Documentation Writer", parent: "[ORG]POD-EPT", type: "AI Agent", filler_kind: "ai", accountable_to: "[ORG]CELL-EPO", accountable_human: "[ORG]HOAC-ACS (the product's owner position, [ORG]CELL-EPO)", test: { id: "TEST-PC-EDW", cases: "13, 33", owner: "[ORG]CELL-EPO" }, ai_in: ["PRD, design, rates, launch record"], ai_out: ["explainer set drafts"], bot: { allowed_actions: ["write the explainer and supporting documents of the product"], ask_first_actions: ["anything outside its role card"] } }
  pods:
    - { code: "[ORG]POD-PCCO", full_name: "Product Core CPO Office", type: "AI Pod", inner_units: ["[ORG]CELL-PIC", "[ORG]CELL-PK", "[ORG]CELL-SK", "[ORG]CELL-PRS", "[ORG]CELL-IPA"], top_cell: "[ORG]CELL-PK", test: { id: "TEST-PC-PCCO", cases: "4, 9, 14, 15, 17, 21, 34, 36" }, ai_in: ["product request", "audit request", "product records"], ai_out: ["intake record", "register row", "audit record", "review brief", "standard version"] }
    - { code: "[ORG]POD-EPT", full_name: "Example Product Team", type: "Product Team", inner_units: ["[ORG]CELL-EPO", "[ORG]CELL-EPM", "[ORG]CELL-EPD", "[ORG]CELL-EPA", "[ORG]CELL-EPEA", "[ORG]CELL-EOCVA", "[ORG]CELL-EDW"], top_cell: "[ORG]CELL-EPO", hoac: "[ORG]HOAC-ACS", label_holder: "[ORG]CELL-EPO", test: { id: "TEST-PC-EPT", cases: "6, 19, 20, 23, 29-33" }, ai_in: ["dispatch from the Chief of Staff"], ai_out: ["the product's records and packages"] }
```

- **Accountability.** The CPO Office Pod, its Cells, the Chief of Staff and each product team are `accountable_to` `[ORG]CELL-CPO`. Each team's AI Cells are `accountable_to` the team's owner position. The AIOC itself and the Chief Product Officer are `accountable_to` the Cell carrying `[ORG]HOAC-TM`.
- **Bots.** Each AI Cell's bot (twelve in the pattern) has its own identity card, its own credential, `never_signs: true`, and its memory sealed on a change of filler (Protocol §10, item 3). The credential IDs in `cards/bots/` are placeholders; the credentials live only in the organisation's vault.
- The Requesting Authority, the positions of each company, the engineering AIOC and Source Lifecycle are not Cells of this AIOC.

**Code checks** (Naming Standard R15 and §5), recorded on 16 October 2026. Each organisation repeats the check of §5.2 against its own register before first use.

| Code | Initials of the full name (R15) | §5.1 | §5.2: no match among this blueprint's codes, nor with `[ORG]AIOC-PC` | §5.3 |
|---|---|---|---|---|
| `[ORG]CELL-CPO` | **C**hief **P**roduct **O**fficer | pass | pass | pass |
| `[ORG]CELL-PCCS` | **P**roduct **C**ore **C**hief of **S**taff ("of" skipped) | pass | pass (distinct from `[ORG]CELL-PCS` of another AIOC) | pass |
| `[ORG]POD-PCCO` / `[ORG]CELL-PIC`, `-PK`, `-SK`, `-PRS`, `-IPA` | Product Core CPO Office / Product Intake Clerk, Portfolio Keeper, Standards Keeper, Product Review Secretary, Independent Package Auditor | pass | pass | pass |
| `[ORG]POD-EPT` / `[ORG]CELL-EPO`, `-EPM`, `-EPD`, `-EPA`, `-EPEA`, `-EOCVA`, `-EDW` | Example Product Team / Example Product Owner, … Example Documentation Writer (pattern codes; each team's codes come from its product's name) | pass | pass | pass |

No code of this blueprint uses the suffix `PC` alone, so no part can be read as the AIOC itself. **UNVERIFIED** against any organisation's unit register; each organisation checks them in its own.

---

## Annex A. The product package and the records of a product's life

Field lists. Every field is filled; "none" is an answer (Protocol §18, item 6.2). A package sent on the product line is frozen and content-addressed: its ID is the hash of its manifest, and the manifest lists every part by hash (card output 1).

### A.1 The package manifest

| Field | Content |
|---|---|
| `package_id` | the SHA-256 of the canonical manifest (content address) |
| `product` | the product's portfolio ID |
| `version` | the package version; a changed package is a new version, never an edit |
| `supersedes` | the package version it replaces, or none |
| `parts` | each part: kind (PRD, feature package, design, copy, explainer reference), path, SHA-256 |
| `acceptance_index` | every acceptance criterion of every feature, by ID |
| `rests_on` | the research record and the sources it cites, by reference |
| `decided_by` | the owner position's code and the decision's reference |
| `companies_and_markets` | the configurations it is for, by reference to the portfolio |
| `audit` | the Independent Package Auditor's record, by reference |

### A.2 The PRD

| Field | Content |
|---|---|
| Problem and customer | who, and what they need, from the research record |
| Goal and measures | each measure with its definition, baseline and target, from a source or a decision, or `not given` |
| Scope | in, and out |
| Requirements | each with ID, statement, source by reference or **New**, priority (must, should, could) |
| Rates and economics | the rates that apply, by reference to their records; the product economics |
| Terms | the product's terms, by reference, including whether a new rate reaches existing deals |
| Languages and markets | every language the product serves, and its direction |
| Risks and open questions | each with its owner position |
| Explainer set | the documents the product needs (A.5) |

### A.3 A feature package

| Field | Content |
|---|---|
| Feature ID and name | |
| The requirement IDs it meets | |
| User stories or jobs | |
| Acceptance criteria | each with ID, a pass condition a tester can check, and its evidence kind |
| States and edge cases | |
| Copy | by reference to A.4 |
| Out of scope | |

### A.4 The design

| Field | Content |
|---|---|
| Flows | each flow, step by step |
| Screens | each screen in every state: default, empty, loading, partial, error, success, permission refused, and offline where the product runs offline |
| Copy | every string in every language served, right to left included where served |
| Design system | its version; each deviation with its reason |

### A.5 The explainer set

The product explainer and its questions and answers; help articles and user guides; partner materials; internal training. Each is a versioned document, filed into Source Lifecycle with the owner position as contributor.

### A.6 The launch record

| Field | Content |
|---|---|
| The package version launched | by `package_id` |
| Checks | package accepted (by criterion); explainers filed; rates set (by record); support ready; configurations per company and market set; terms reviewed |
| Decision | the owner position's, with its date |

### A.7 The retirement record

| Field | Content |
|---|---|
| The outcome | the review that decided `retire`, by reference |
| Closing steps | rates closed (by record); explainers withdrawn in Source Lifecycle; customer communications sent; the team retired under `retire-unit` |
| Decision | the Chief Product Officer's, with its date |

## Annex B. The rate record

| Field | Content |
|---|---|
| `rate_id` | stable across versions |
| `version` | increasing; a change is a new version, never an edit |
| `product` | the product's portfolio ID |
| `applies_to` | the companies and markets, by reference |
| `value` | the price, fee or rate, with its unit |
| `effective_from` | the date it takes effect |
| `reason` | why it changed |
| `replaces` | the version it replaces, or none |
| `existing_deals` | whether it reaches existing deals, with the clause of the product's terms that says so |
| `decided_by` | the owner position's code and the decision's reference (and the `commit-money` signature, where set) |
| `hash` | the SHA-256 of the record, checked on read-back |

A reversal is a new version whose value is an earlier version's value, with its own reason (Protocol §18, item 7).

## Annex C. The portfolio register

| Field | Content |
|---|---|
| `product` | the product's ID and name |
| `category` | one category of the organisation's own record |
| `category_kind` | one of: product family (grouped by the customer's principal destination), platform (shared capabilities every product uses; a capability is never a product), company category (the products of one company that stand apart from the families), AI Systems (assistants, agents, agent-run websites, back offices, internal panels and internal tools that are not sold) (Protocol §18, item 4) |
| `owner_position` | one position code, holding no other product |
| `team` | the product team's Pod code |
| `stage` | P1 to P8 (§5.0), or retired |
| `configurations` | one row per company and market that offers it; never a copy of the product |

Which categories an organisation has, and what each holds, is the organisation's own record and never appears in the Library (Protocol §18, item 4).

## Annex D. What this AIOC never does

1. Write code, technical design or infrastructure, or set the build plan or its dates.
2. Speak to a builder or to the code host, or send product work other than on the product line.
3. Send an incomplete package, or one the Independent Package Auditor has not passed.
4. Copy a product for a company instead of configuring it.
5. Record a capability as a product.
6. Give one owner position two products, or a product two owner positions, or hand a stage of a product's life to another team.
7. Change a rate by a code release, or without an effective date and a reason.
8. Invent a figure, a target or a price.
9. Name a person, or read who occupies a position.
10. Let an AI decide, accept or sign.
11. Put an organisation's products, categories or rates into the Library.

*`[ORG]AIOC-PC` mother blueprint v0.1.0 · Powered by 49GAION*
