# Contributing

Thanks for considering a contribution to Awesome Morpheus!

## Guidelines

### Morpheus Plugins

- **Scope**: Only community plugins for Morpheus Data belong here, i.e. plugins that carry neither the "Official" nor "Partner" designation on the [Morpheus Marketplace](https://share.morpheusdata.com). Official and partner plugins should not be added.
- **One line per entry**: `**Name** - Short, factual description. [Marketplace](link) · [Source](link)`
- **Sort alphabetically** within a category.
- **Working links only**: Link to the plugin's Marketplace page. Include its public source repository if one exists; otherwise note that source is not publicly available.
- **No duplicates**: Check existing entries before adding a new one.
- **New categories**: Only add a new category if an entry doesn't reasonably fit an existing one, and add it to the table of contents.

### Copilot Agents & Skills

Copilot agents and skills work fundamentally differently from plugins: they run client-side in a Copilot client (CLI/IDE) rather than inside a Morpheus instance, and interact with Morpheus externally (e.g. via its REST API or CLI):

- **Scope**: Must interact with Morpheus specifically and be usable with GitHub Copilot.
- **Agents**: Add a single `<name>.agent.md` file to [`agents/`](agents/) with YAML frontmatter (`name`, `description`, `tools`) and a system prompt.
- **Skills**: Add a folder to [`skills/`](skills/) named after the skill, containing a `SKILL.md` (plus any bundled assets/scripts).
- List new entries under the README's [Copilot Agents & Skills](README.md#copilot-agents--skills) section.
- No official warranty or endorsement is implied; the same [disclaimer](README.md#disclaimer) applies.

## Submitting

1. Fork the repository.
2. Add your entry following the guidelines above.
3. Open a pull request with a short description of the plugin and why it belongs on the list.

All submissions are reviewed against the criteria above before merging.
