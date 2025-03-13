# Filozoff/action-make-tag

A simple GitHub Action that creates and push git tag using GitHub API.

## Usage

### Inputs

- `tag`: Derived data path (optional). Default: `./.build`.
- `token`: GitHub (optional). Default: `GITHUB_TOKEN`.

### Setup

```yaml
jobs:
  make-tag:
    runs-on: linux-latest # You can use any runner with OS which supports sh scripts
    steps:
      - name: Make tag
        uses: Filozoff/action-make-tag@v1
        with:
          tag: "1.1.2"
          token: "..."
```

## Limitations

- Only works with runners which supports sh scripts

## License

[MIT License](LICENSE)
