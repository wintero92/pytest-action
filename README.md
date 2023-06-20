# pytest-action

## How to use

```
jobs:
  pytest:
    runs-on: ubuntu-latest

    steps:
      - name: Check-out
        uses: actions/checkout@v3
        with:
          fetch-depth: 1

      - name: Pytest
        uses: wintero92/pytest-action@v1
        with:
          package-name: wopee_agent
          min-cov: 0
          retention-days: 10
```

## Inputs

See `action.yaml` for possible inputs.