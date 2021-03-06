# react-packages

Meteor packages for a great React developer experience

[Read the guide.](http://react-in-meteor.readthedocs.org/en/latest/)

## Development prerequisites

**These prerequisites are for developing these packages, not for using them.**

* node@8
* npm@5

### Running the docs site locally

1. Install `mkdocs` with `pip`
2. Run `mkdocs serve` from the root of the repository

### Linting

Run

```
npm run lint
```

Note this does not yet all lint. Working on it.

### Testing

Due to difficulties in testing packages with "peer" NPM dependencies, we've worked around by moving package tests into harness test apps. You can find them in `tests/`.

### Publishing

Due to the dependency graph, the order these packages are published in can be
important.

In order to simplify the process, the `./publish-packages.sh` script can be 
used to automatically bump package versions and publish the packages in the
correct order.

> This is a shortcut to the script in `scripts/publish-packages/index.js`.

