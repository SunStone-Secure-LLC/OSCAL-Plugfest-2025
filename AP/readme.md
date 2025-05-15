## Referencing the SSP Locally

Some of the files in this directory (e.g., SAP, POA&M) are derived from a System Security Plan (SSP) and include a reference to it in their `back-matter` or `import-ssp` section.

If you download and test these files locally, you may need to update the reference to use a local file URI.

### 🔧 Example Usage

```json
"href": "file:///path/to/your/ssp/valid_oscal_ssp_1.json"
```

Replace /path/to/your/ssp/ with the actual location on your machine.
For example:
```json
"href": "file:/Users/<your-username>/Documents/OSCAL-Plugfest-2025/SSP/Valid/valid_oscal_ssp_1.json"
```
