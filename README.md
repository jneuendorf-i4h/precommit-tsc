TypeScript Check for Precommit
===============

TSC for pre-commit.

For pre-commit see: https://github.com/pre-commit/pre-commit

For Typescript and TSC cli see: https://github.com/microsoft/TypeScript/

### Using prettier with pre-commit

Add this to your `.pre-commit-config.yaml`:

```yaml
  - repo: https://github.com/mohsentaleb/precommit-tsc
    rev: 'v1.0.0'
    hooks:
      - id: tsc
```

By default, files with extension `.ts` and `.tsx` are passed to `tsc`, if you want to add or remove to this list, use `types` / `types_or` / `files` directives or read more [here](Filtering files with types):

```yaml
    -   id: tsc
        types_or: [ts, tsx, jsx]
```
