# GraphQL Pre-Commit Hooks

Two simple hooks for linting and formatting GraphQL schemas.

## Usage

Set-up your project with https://pre-commit.com/ and add the following
lines to your configuration file:

    - repo: https://github.com/leehambley/pre-commit-graphql.git
      rev: master
      hooks:
      - id: graphql-schema-linter
      - id: format-graphql

Any files ending with `.graphql` which are staged in Git's index will be run through these two filters.

## Heads-up

`format-graphql` is quite aggressive in sorting/reordering keys and types/etc, check more in the docs:

- https://www.npmjs.com/package/format-graphql
