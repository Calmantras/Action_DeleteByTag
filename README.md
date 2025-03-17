# Delete Release Assets By Tag

GitHub Action to delete all assets from a release identified by its tag name.

## Development

```bash
# Install dependencies
npm install

# Bundle for production (creates dist/index.js)
npm run bundle
```

## Inputs

- `asset_tag`: Tag name of the release to remove assets from (required)
- `asset_owner`: Owner of the repository (optional, defaults to context owner)
- `asset_repo`: Name of the repository (optional, defaults to context repository)

## Usage

```yaml
steps:
  - uses: Calmantras/Action_DeleteByTag@v1.0
    with:
      asset_tag: v1.0.0
      # Optional parameters:
      # asset_owner: username
      # asset_repo: reponame
```