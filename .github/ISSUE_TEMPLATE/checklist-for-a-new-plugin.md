---
name: Checklist for a new plugin
about: This template describes the features that plugins should have
title: Checklist for a plugin
labels: plugin_checklist
assignees: ''

---

This plugin is developed at: 

Required: the plugin is -

- [ ] posted to pypi
- [ ] shows up properly after install with `info -v`
- [ ] has correct installation requirements specified in `pyproject.toml`
- [ ] is listed in sourmash-mixers `pyproject.toml` and `README.md`

Strongly suggested:

- [ ] plugin has a basic README
- [ ] if a script, `scripts` output is a good single line
- [ ] `sourmash` is in the repository tags

Upgrading your plugin:

- [ ] plugin code from template no longer has any 'xyz' strings
- [ ] README contains example command lines, output, and/or screenshots
- [ ] plugin has good default output for basic usage, `-h/--help`, and epilog
- [ ] plugin has some automated tests
- [ ] automated tests run on PRs and commits
- [ ] `-q/--quiet` and `-d/--debug` suppress and produce output appropriately
- [ ] plugin has sourmash listed 

The long haul:

- [ ] plugin has automated tests with good code coverage
