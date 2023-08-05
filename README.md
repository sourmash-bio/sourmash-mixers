# sourmash-mixers

[![PyPI version](https://badge.fury.io/py/sourmash-mixers.svg)](https://badge.fury.io/py/sourmash-mixers)

`sourmash-mixers` is a meta-package to install a number of useful
[sourmash plugins](https://sourmash.readthedocs.io/en/latest/command-line.html#using-sourmash-plugins)!

Our intention is that all "suitably mature" sourmash plugins will be
available via `sourmash-mixers`, at least for now. "Maturity" rubrics
are defined
[here](https://github.com/ctb/sourmash-mixers/blob/main/.github/ISSUE_TEMPLATE/checklist-for-a-new-plugin.md), but it's an evolving criteria...

The list of plugins installed by `sourmash-mixers` is available [in `pyproject.toml` under **dependencies**](https://github.com/ctb/sourmash-mixers/blob/main/pyproject.toml) - the list includes:

* [a command-line plugin to produce 2- and 3-way Venn diagrams of sketches](https://github.com/sourmash-bio/sourmash_plugin_venn)
* [a command-line plugin to sketch many samples or genomes](https://github.com/sourmash-bio/sourmash_plugin_sketchall)
* [a command-line plugin to download NCBI genomes by accession](https://github.com/ctb/get-some-ncbi-genomes/)
* [a command-line plugin to filter hashes by presence/absence in multiple samples](https://github.com/ctb/sourmash_plugin_commonhash)
* [a command-line plugin to plot abundance histograms](https://github.com/ctb/sourmash_plugin_abundhist)

## Installation

This command:
```
pip install sourmash-mixers
```
will install the latest version of `sourmash-mixers`.

## Usage

Command-line plugins are available under:
```
sourmash scripts
```
and detailed usage information for each plugin command can be seen with
```
sourmash scripts <command> -h
```
e.g. `sourmash scripts sketchall -h`.

You can list all installed plugins with:
```
sourmash info -v
```

## Developer information

If you're interested in developing your own plugin, or updating an
existing plugin, please see
[sourmash plugins via Python entry points](https://sourmash.readthedocs.io/en/latest/dev_plugins.html). A template repository is available there for
people who want to just get started writing code! Or you can get started
with any of the plugins described above!

For questions, comments, and help writing and testing plugins, please
file issues
[over on sourmash-bio/sourmash](https://github.com/dib-lab/sourmash/issues)
and/or
[visit our gitter/matrix channel](https://github.com/sourmash-bio/sourmash/issues/1686).

Some back story on plugins - their motivation, and their
implementation - can be found
[in this blog post](http://ivory.idyll.org/blog/2023-sourmash-plugins-first-effort.html).

If you're interested in adding your own plugin to sourmash-mixers
specifically, please create a new issue with "Checklist for a new plugin"
and fill it out as you can, and then ask for more instructions on that issue!
