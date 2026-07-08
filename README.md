# AI Code Lint

Catch common AI-generated code smells in Python before they merge.

## What it does
Scans `.py` files for hallucinated/non-existent API calls, I/O without error handling, overly complex comprehensions, and import-count bloat, then reports findings. In `strict` mode it fails the workflow when issues are found.

## Usage
```yaml
- uses: CodeGero/ai-lint@v1
  with:
    path: '.'
    strict: 'false'
```

## Inputs
| Input | Required | Default | Description |
|---|---|---|---|
| `path` | no | `.` | Directory to scan. |
| `strict` | no | `false` | Fail the workflow when issues are detected. |

## Checks performed
- Hallucinated APIs (calls that are not imported/defined)
- I/O operations without `try/except`
- Overly nested/complex comprehensions
- Excessive import counts per module

## License
MIT — free to use. Premium support via [Gumroad](https://kryptorious.gumroad.com/l/jbvet).
