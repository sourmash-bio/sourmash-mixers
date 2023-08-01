---
name: Checklist for a new plugin
about: This template describes the features that plugins should have
title: Checklist for a plugin
labels: plugin_checklist
assignees: ''

---

Absolute requirements for a plugin:
- [ ] posted to pypi
- [ ] shows up properly after install with `info -v`
- [ ] installation requirements are correct

Minimal requirements:

- [ ] plugin has a basic README
- [ ] if a script, `scripts` output is a good single line

Upgrading your plugin:

- [ ] plugin code from template no longer has any 'xyz' strings
- [ ] README contains example command lines, output, and/or screenshots
- [ ] plugin has good default output for basic usage, `-h/--help`, and epilog
- [ ] plugin has some automated tests
- [ ] automated tests run on PRs and commits
- [ ] `-q/--quiet` and `-d/--debug` suppress and produce output appropriately

The long haul:

- [ ] plugin has automated tests with good code coverage
