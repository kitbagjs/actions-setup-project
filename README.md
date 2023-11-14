# actions-setup-project
## Details
A Github Action that sets up a NodeJS environment, checks out the repository, and installs dependencies.

## Usage
```yaml
name: Tests
on: [ pull_request ]
jobs:
  types:
    name: Type Validation
    runs-on: ubuntu-latest

    steps:
      - name: Setup
        id: setup
        uses: kitbagjs/actions-setup-project@main

      - name: Validate types
        run: npm run types
```
