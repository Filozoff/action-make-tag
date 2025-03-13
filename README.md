# Filozoff/action-make-tag

A simple GitHub Action that creates and push git tag using GitHub API.

## Usage

### Inputs

- `commit-sha`: Commit sha (optional). Default: `github.sha`.
- `tag`: Tag name.
- `token`: Authorization token (optional). Default: `GITHUB_TOKEN` env.

### Setup

```yaml
jobs:
  make-tag:
    runs-on: linux-latest
    steps:
      - name: Make tag
        uses: Filozoff/action-make-tag@v1
        with:
          commit-sha: ${{ github.sha }}
          tag: "1.1.2"
          token: "..."
```

## Limitations

- None

## License

[MIT License](LICENSE)
