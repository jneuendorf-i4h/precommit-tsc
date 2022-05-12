prettier mirror
===============

Mirror of prettier package for pre-commit.

For pre-commit see: https://github.com/pre-commit/pre-commit

For Typescript and TSC cli see: https://github.com/microsoft/TypeScript/


### Using prettier with pre-commit

Add this to your `.pre-commit-config.yaml`:

```yaml
-   repo: https://github.com/mohsentaleb/precommit-tsc
    rev: ''  # Use the sha / tag you want to point at
    hooks:
    -   id: tsc
```

By default, all files are passed to `tsc`, if you want to limit the
file list, adjust `types` / `types_or` / `files`:

```yaml
    -   id: prettier
        types_or: [ts, tsx]
```
