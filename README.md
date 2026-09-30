# RestoCalc rules

Public, machine-readable rules data (tax rates, service charge norms, minimum wages, statutory contributions and similar) used by the RestoCalc apps. Every value lists its official source, effective date and last-verified date.

The apps ship with a built-in copy and download updates from this repository. Values are checked monthly against official sources.

This data is provided for estimates only and is not tax or legal advice.

## Files

- `rules.json`: the rules the apps download (`rulesVersion`, per-country values with `sources`, `effective` and `verified` dates).
- `rules.schema.json`: the JSON Schema `rules.json` must pass.

Apps only accept a download that is newer than their copy, uses the same schema version and passes validation, so a bad file is ignored rather than applied.
