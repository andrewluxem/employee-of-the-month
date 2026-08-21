# employee-of-the-month

Designs a recurring recognition program and organizes nominations without selecting a winner.

It produces:

- **Employee of the Month Program and Nomination Review:** a working artifact built from supplied facts, labeled inference, and visible missing fields.

It executes the [Employee of the Month playbook](https://www.andrewluxem.com/playbooks/employee-of-the-month). The playbook teaches the framework. This skill runs it and returns a working artifact.

**Static by construction: no dependencies, executable code, telemetry, network calls, remote instructions, auto-update, scheduled work, or background behavior.** It reads only the files in its own skill folder. Nothing happens until a user or agent invokes it.

## Install

Clone and copy the skill into Claude Code:

```bash
git clone https://github.com/andrewluxem/employee-of-the-month.git
cp -r employee-of-the-month/skills/employee-of-the-month ~/.claude/skills/
```

For Codex, copy the same complete folder to the Codex skills directory:

```bash
cp -r employee-of-the-month/skills/employee-of-the-month ~/.codex/skills/
```

Or install it as a Claude Code plugin:

```text
/plugin marketplace add andrewluxem/employee-of-the-month
/plugin install employee-of-the-month@employee-of-the-month
```

For clients that install from an archive, use the versioned [employee-of-the-month v1.0.0 ZIP](https://www.andrewluxem.com/downloads/employee-of-the-month-v1.0.0.zip).

## Invoke it

```text
Design an employee of the month program and nomination review
Use the employee-of-the-month skill.
```

Naming the skill is always valid: `use the employee-of-the-month skill`.

## Files

```text
.claude-plugin/
  plugin.json
  marketplace.json
skills/employee-of-the-month/
  assets/employee-of-the-month-program-template.md
  LICENSE.md
  meta.yaml
  references/nomination-review-standard.md
  SKILL.md
README.md
LICENSE
```

The complete canonical package is copied under `skills/employee-of-the-month/`, including every asset, reference, test prompt, source note, changelog entry, and license file present in the source.

## Versioning

Plugin installation is version-pinned. When behavior changes, update the version consistently in `SKILL.md`, `meta.yaml`, `.claude-plugin/plugin.json`, and `.claude-plugin/marketplace.json`, then add a changelog entry. Reinstalling is an explicit update; this repository never auto-updates itself.

## License

MIT. See [LICENSE](LICENSE). The canonical skill folder carries the same authorization in [skills/employee-of-the-month/LICENSE.md](skills/employee-of-the-month/LICENSE.md).

---

## More playbooks

This skill packages one playbook from the free library at [github.com/andrewluxem/playbooks](https://github.com/andrewluxem/playbooks). Every playbook is free to read, with no email required.
