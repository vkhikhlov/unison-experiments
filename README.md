# Unison experiments

This repo contains some of my experiments with the [Unison](http://unisonweb.org) language.

## Installation

From the Unison Codebase Manager (`ucm`) prompt:

```
.> pull https://github.com/vkhikhlov/unison-experiments
```

This will install all libraries under namespace external and fetch some unison definitions under namespace .trunk.

To view what's available prompt:

```
.> cd .trunk
.trunk> ls
```

To run main program prompt:

```
.trunk> run main
```

## Refactoring and code updates workflow

```
.> fork .trunk .prs.experiments._mything
.> cd .prs.experiments._mything
.prs.experiments._mything> ls
.prs.experiments._mything> edit someDefinition
.prs.experiments._mything> update
.prs.experiments._mything> diff.namespace .trunk .prs.experiments._mything
.prs.experiments._mything> view 1-4
.prs.experiments._mything> merge .prs.experiments._mything .trunk
.prs.experiments._mything> cd .trunk
.trunk> push
```

## Contributing

This repository follows the conventions in [this document](https://www.unisonweb.org/docs/codebase-organization/) and I recommend reading that document, in particular [this section on creating and managing pull requests](https://www.unisonweb.org/docs/codebase-organization/#day-to-day-development-creating-and-merging-pull-requests).
