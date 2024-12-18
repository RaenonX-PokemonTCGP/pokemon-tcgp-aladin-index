# pokemon-tcgp-aladin-index

Stores the aladin index files.

Also stores the GitHub Actions workflows for initiating the auto datamining.

## Development

For local GitHub actions workflow testing, run the following command with nektos act installed.

```powershell
act `
    -P windows-latest=-self-hosted `
    -W .\.github\workflows\auto-mine-asset.yml `
     --secret-file .secrets-assets
```

```powershell
act `
    -P windows-latest=-self-hosted `
    -W .\.github\workflows\auto-mine-masterdata.yml `
     --secret-file .secrets-masterdata
```