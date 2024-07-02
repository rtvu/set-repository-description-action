# SET-REPOSITORY-DESCRIPTION-ACTION

GitHub Action to set repository's description.

## Usage

``` yaml
name: Set repository description
uses: rtvu/set-repository-description-action@v1.0.0
with:
  description: Description of repository
  repository: ${{ github.repository }}
  token: ${{ secrets.REPOSITORY_PAT }}
```

## Inputs

| Name          | Description                                         | Required |
| ------------- | --------------------------------------------------- | -------- |
| `description` | Description of repository                           | `true`   |
| `repository`  | Name of repository with format <OWNER>/<REPOSITORY> | `true`   |
| `token`       | GitHub token                                        | `true`   |
