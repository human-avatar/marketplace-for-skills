# marketplace-4-skills

A [Claude Code plugin marketplace](https://code.claude.com/docs/en/plugin-marketplaces) of skill packs — structured, invokable thinking and decision-making frameworks you can run as slash commands.

## Plugins

| Plugin | What it does |
| --- | --- |
| [`skills-for-humanity`](https://github.com/human-avatar/skills-for-humanity) | Thinking skills for Claude Code — logic, ethics, creativity, decision-making, systems thinking, communication, and more. |
| [`skills-for-agriculture`](https://github.com/human-avatar/skills-for-agriculture) | Decision-making and guidance skills for farmers, growers, and land stewards — regenerative agriculture, soil health, water, livestock, pests, seasons, and more. |

## Install

Add the marketplace, then install the plugins you want:

```shell
/plugin marketplace add human-avatar/marketplace-for-skills
/plugin install skills-for-humanity@marketplace-4-skills
/plugin install skills-for-agriculture@marketplace-4-skills
```

Browse and manage everything interactively with:

```shell
/plugin
```

## Updating

When the marketplace catalog changes, refresh your local copy:

```shell
/plugin marketplace update marketplace-4-skills
```

## License

MIT — see [LICENSE](LICENSE). Individual plugins are licensed in their own repositories.
