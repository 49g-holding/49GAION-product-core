# DR-0001 · The mother repository of Product Core, and its first mother blueprint

- **Date:** 2026-10-16
- **Decided by:** the governing seat (GOV) of 49GAION
- **Sources:** `49GAION/DR-0024` (a mother repository for a Library part whose first instance holds an organisation's data); the Protocol section Product Core (§18) and the part card `product-core.part-card.json` v1, proposed on 15 October 2026; `49GAION/DR-0019` (the Library register) and `DR-0021` (mother and instance)

## Decision

1. **This repository.** `github.com/49g-holding/49GAION-product-core`, public, is the mother repository of the Library part 49GAION Product Core. It holds the mother blueprint only, laid out and checked as a writing repository.
2. **The first mother blueprint.** `blueprint/PC-BLUEPRINT.md` `v0.1.0`, draft, on the 49GAION AIOC template at `1abae80`, from Protocol §18 and the part card v1. It adds the CPO Office's parts, the product team pattern, the eight stages with their gates, and the field lists of the product package, the rate record and the portfolio register; each rule cites §18 or is marked **New**.
3. **No organisation's data.** No product, category, price or company of any organisation is written here; the first instance keeps its own in its private home.
4. **The fixed test.** TEST-PC v1, 48 cases, every one `NOT_RUN`, with TEST-PRODUCT-CORE v1 kept unchanged as cases 1 to 13 (`tests/TEST-PC.md`).
5. **The Library pin.** Once merged, this text is pinned in `49GAION-protocol` `library/README.md` by repository, path, version, commit and SHA-256.

## Not decided here

Everything in blueprint §13 stays open, including the money and legal rows (H-03, H-04).

*Powered by 49GAION*
