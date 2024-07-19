# SET-REPOSITORY-DESCRIPTION-ACTION

GitHub Action to set repository's description.

## Usage

``` yaml
name: 'Set repository description'
uses: rtvu/set-repository-description-action@v1
with:
  description: 'Description of repository'
  token: ${{ secrets.REPOSITORY_TOKEN}}
```

## Inputs

| Name          | Description                                           | Default                    |
| ------------- | ----------------------------------------------------- | -------------------------- |
| `description` | Description of repository                             |                            |
| `repository`  | Name of repository with format `<OWNER>/<REPOSITORY>` | `${{ github.repository }}` |
| `token`       | GitHub token[^1]                                      |                            |

[^1]: Cannot use `GITHUB_TOKEN`. Does not have proper permissions.
