# 49GAION Product Core · the mother blueprint

The mother repository of the Library part **49GAION Product Core**. In an `[ORG]AION`, the part is the AIOC `[ORG]AIOC-PC`. Public. It holds the mother blueprint only, for any organisation, with no organisation's data: no product, no category, no price, no company (`49GAION/DR-0024`; Naming Standard R9, addition 4).

> **Reading (49GAION DR-0041).** The complete definition of 49GAION, approved by its governing seat on 25 October 2026, is `49GAION-FRAMEWORK.md` in `github.com/49g-holding/49GAION`. Where this repository differs from it, the definition governs, and this text is read with it. Every rule here that names `[ORG]AIOC-OCO` or the human hub reads as the Top Management Group, the hub of the operation, human and AI. The panel is the organisation's own code interface, and the AI chat workspace is its back office. The readings are in [`decisions/DR-0004`](decisions/DR-0004-the-readings-of-dr-0041.md). Nothing here is removed.

Product Core is the organisation's one product division, shared by every company it runs. It owns the what and the why of every product for the product's whole life; the engineering AIOC owns the how and the when. Its head office is the CPO Office. Each product has one team for every stage of its life: one owner position and AI members by function (Protocol §18).

The one-page summary is at the top of the blueprint.

## What is here

| Path | What it is |
|---|---|
| [`MANDATE.md`](MANDATE.md) | the mandate, `v0.2.0`, proposed: the organisation (the CPO Office, Discovery, the Design and Brand Studio, the categories, a team of twelve agents per product), the 47 duties, the sixteen processes, the human acts and how a seat hands them to its COS, default times and stand-ins, making any position human, and the paths with the human hub, the engineering AIOC, the engine division and the marketing division. Where it differs from the blueprint, it governs (`decisions/DR-0003`) |
| [`blueprint/PC-BLUEPRINT.md`](blueprint/PC-BLUEPRINT.md) | the mother blueprint, `v0.1.1`, on the 49GAION AIOC template |
| [`tests/TEST-PC.md`](tests/TEST-PC.md) | the fixed test, TEST-PC v1: 48 cases, every one `NOT_RUN`, keeping the Library's TEST-PRODUCT-CORE v1 as cases 1 to 13 |
| [`cards/`](cards/) | the unit cards of its Pods and Cells, and the bot identity cards, generated from blueprint §17 |
| [`decisions/`](decisions/) | the decision records of this repository |
| [`upstream/PROPOSALS.md`](upstream/PROPOSALS.md) | drafts of proposals to 49GAION, not yet proposed |
| [`tools/make_cards.py`](tools/make_cards.py) | generates and checks the cards (case 46) |

## Mother and instance

- **The Library pins this text** by repository, path, version, commit and SHA-256 (`49GAION-protocol`, `library/README.md`). A new version reaches the Library only by a pull request that moves the pin.
- **Each organisation makes its own instance** from it: its writing repository `<org>aioc-pc`, private where it holds the organisation's products, categories and rates, with the `<organisation>`, `<org>` and `<filled>` values set (blueprint §0, §2.1, §15), and one product team per product made from the pattern of §17. The organisation's values never come back here.

## Checks

**The Protocol pin.** The checks are the one set of checks of the Library repositories, the action `library-checks` of `49GAION-protocol`, run at the commit in `PROTOCOL-PIN`, which also gives the schemas and the `no-org-names` scanner they read, never at `main`, so a change in the Protocol changes nothing here until this repository moves the pin by pull request.

On every pull request and on main (`.github/workflows/checks.yml`):

```
python3 tools/make_cards.py <49GAION-protocol>/spec/schemas      # 0 errors; the committed cards are the generated cards
bash <49GAION-protocol>/.github/scripts/no-org-names.sh          # no organisation name, host or prefixed code
```

and no Persian or Arabic-script character in any tracked file.

## Owner and licence

- **Owner and licence.** The copyright holder, and the licences of the texts (CC BY 4.0, credit "Powered by 49GAION") and of the code (Apache-2.0), are in [`LICENSE.md`](LICENSE.md).

*Powered by 49GAION*
