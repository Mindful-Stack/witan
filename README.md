# Witan

> *Witan* (Old English): an assembly of wise advisors. The Anglo-Saxon king's council, drawing on the wisdom of bishops, ealdormen, thegns, and reeves to deliberate on matters of the realm. Etymologically the root of *wisdom*, *witness*, and *wit*.

The **Witan** is [Mindful Stack](https://github.com/Mindful-Stack)'s family of AI dev tools — a council where each member is a specialist in its craft.

This repo is the **Claude Code plugin slice** of that council: a [Claude Code marketplace](https://docs.claude.com/en/docs/claude-code/plugin-marketplaces) that catalogs the Witan members which ship as plugins. Other members (orchestrators, CLIs, services) are distributed separately — see [The wider Witan](#the-wider-witan) below.

## Add the marketplace

Inside Claude Code:

```text
/plugin marketplace add Mindful-Stack/witan
```

## Plugin members

| Plugin | Role | Status |
|--------|------|--------|
| [lore](https://github.com/Mindful-Stack/lorekeeper) | Lorekeeper — keeper of knowledge: domain context, pattern lookup, PR review | Available |

Install a member:

```text
/plugin install lore@witan
```

## The wider Witan

Not every Witan member is a Claude Code plugin. Some are independent applications that sit alongside Claude Code rather than inside it.

| Member | Form | Role | Status |
|--------|------|------|--------|
| reeve | Orchestrator app | Steward of the project — coming soon | Planned |

Apps are distributed via their own repos and release channels — see each member's README for setup. They share the medieval-role naming and the Mindful Stack ethos, but not this marketplace's install path.

## Why a council?

Each member does one thing well. Splitting capabilities into focused tools means each evolves independently — a new release of `lorekeeper` doesn't require a `reeve` update.

For Claude Code plugins, this marketplace is the single registry: add it once, install members as you need them.

## Convene the council *(coming soon)*

Once a second member ships, this repo will gain a one-command setup that installs every Witan member, wires them together, and writes the config files they expect:

```bash
# planned, not yet implemented
./scripts/setup.sh
```

Until then, install members individually via the marketplace (plugins) or each member's own README (apps).

## Adding a plugin to the marketplace

1. Build and publish your plugin to its own GitHub repo (with `.claude-plugin/plugin.json`).
2. Open a PR against this repo adding an entry to `.claude-plugin/marketplace.json`.
3. Members are reviewed for fit with the council's character — focused, well-tested, documented.

## Adding a non-plugin member to the wider Witan

Not yet codified — open an issue if you have a candidate.

## Licence

Marketplace metadata is unlicensed (effectively public domain). Each plugin in the council carries its own licence — see the linked repos.
