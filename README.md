# Witan

> *Witan* (Old English): an assembly of wise advisors. The Anglo-Saxon king's council, drawing on the wisdom of bishops, ealdormen, thegns, and reeves to deliberate on matters of the realm. Etymologically the root of *wisdom*, *witness*, and *wit*.

The Witan is the [Mindful Stack](https://github.com/Mindful-Stack) marketplace for Claude Code — a council of focused plugins, each a specialist in its craft. Add the marketplace once, install members as you need them.

## Add the marketplace

Inside Claude Code:

```text
/plugin marketplace add Mindful-Stack/witan
```

## Members

| Plugin | Role | Status |
|--------|------|--------|
| [lorekeeper](https://github.com/Mindful-Stack/lorekeeper) | Keeper of knowledge — domain context, pattern lookup, PR review | Available |
| reeve | Steward of the project — coming soon | Planned |

Install a member:

```text
/plugin install lorekeeper@witan
```

## Why a council?

Each plugin does one thing well. The Witan brings them together under a single registry so you can compose your own retinue without juggling marketplace URLs.

Members evolve independently — a new release of `lorekeeper` doesn't require a `reeve` update. The marketplace pins versions when stability matters and tracks `main` when you want the bleeding edge.

## Adding a plugin

1. Build and publish your plugin to its own GitHub repo (with `.claude-plugin/plugin.json`).
2. Open a PR against this repo adding an entry to `.claude-plugin/marketplace.json`.
3. Members are reviewed for fit with the council's character — focused, well-tested, documented.

## Licence

Marketplace metadata is unlicensed (effectively public domain). Each plugin in the council carries its own licence — see the linked repos.
