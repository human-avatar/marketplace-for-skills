# marketplace-for-skills

A [Claude Code plugin marketplace](https://code.claude.com/docs/en/plugin-marketplaces) from [**human-avatar**](https://github.com/human-avatar) — a catalog of **skill packs** that give Claude structured, expert-grade methodologies you can run as slash commands.

> **Building with AI. Staying human.**

## About the project

human-avatar packages the *how* of human expertise — not generic advice — into Claude Code skills. Each skill encodes a complete procedure drawn from the people who defined a field: a defined problem type, a sequence of moves, and a structured output. The aim is to keep human judgment, rigor, and craft at the center while working with AI, rather than handing the thinking over to it.

This marketplace is the front door to those packs. Add it once, then install whichever packs you want; updates flow through automatically as the catalog grows.

## What's in this marketplace

Each entry below is a self-contained plugin (its own repo) bundling dozens of related skills. More packs will be added over time.

### 🧠 [`skills-for-humanity`](https://github.com/human-avatar/skills-for-humanity)

Structured reasoning methodologies from history's most rigorous thinkers — de Bono, Meadows, Tetlock, Kahneman, Sun Tzu, Rawls, Shannon, and more — packaged as runnable skills. Roughly five clusters:

- **Think Sharper** — logic, probability, decision-making, constraints, game theory, epistemology, economics
- **Think Differently** — creativity, analogy, play, evolution, design
- **Think About People** — communication, ethics, narrative, psychology, writing, identity
- **Think in Time & Systems** — systems, strategy, history, networks, resources, ecology
- **See More Clearly** — aesthetics, sensory observation

Start with `/s4h` and describe your situation — it routes you to the right methodology automatically.

### 🌱 [`skills-for-agriculture`](https://github.com/human-avatar/skills-for-agriculture)

Decision-making and guidance skills for farmers, growers, and land stewards, grounded in practitioner knowledge and the soil food web — covering regenerative agriculture, soil health, water, livestock, pests, and seasons. Sustainability-biased by default, but transition-aware: it meets you wherever you are on the conventional-to-regenerative spectrum.

Start with `/s4ag` and describe your farm decision.

## Install in Claude Desktop

> Plugins are a **Claude Code** feature. These steps work in the Claude Code desktop app — and identically in the terminal and IDE extensions, since they all share the `/plugin` system. (This is separate from the standalone Claude chat app's connectors.)

**1. Add the marketplace.** In a Claude Code session, run:

```shell
/plugin marketplace add human-avatar/marketplace-for-skills
```

This registers the catalog so you can browse it. Nothing is installed yet.

**2. Open the plugin manager and browse.** Run:

```shell
/plugin
```

Use **Tab** to move between the **Discover**, **Installed**, **Marketplaces**, and **Errors** tabs. On the **Discover** tab you'll see `skills-for-humanity` and `skills-for-agriculture`. Press **Enter** on a plugin to see exactly what it adds (commands, skills, context cost) before installing, and to choose an install scope (user / project / local).

**3. Or install directly from the prompt:**

```shell
/plugin install skills-for-humanity@marketplace-for-skills
/plugin install skills-for-agriculture@marketplace-for-skills
```

**4. Activate.** Run `/reload-plugins` (or restart Claude Code). Skills are namespaced under each pack:

```shell
/s4h        # skills-for-humanity router
/s4ag       # skills-for-agriculture router
```

## Updating

When the catalog changes, refresh your local copy:

```shell
/plugin marketplace update marketplace-for-skills
```

To remove the marketplace (this also uninstalls plugins installed from it):

```shell
/plugin marketplace remove marketplace-for-skills
```

## License

MIT — see [LICENSE](LICENSE). Each plugin is licensed in its own repository.
