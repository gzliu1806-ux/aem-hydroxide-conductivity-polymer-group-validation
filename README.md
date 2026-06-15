# Polymer-group validation of reported hydroxide conductivity in AEMs

This repository contains the public code and summary-data release for the manuscript:

**Polymer-group validation of reported hydroxide conductivity in anion exchange membranes**

The files support inspection of the public schema, polymer-group validation logic, row-wise control path, descriptor-family comparison pattern, reported summary metrics, and figure/source maps used with the manuscript.

## Contents

- `Supplementary_Data_1.xlsx`: public summary validation tables, field definitions, curation rules, and response-selection summaries.
- `Supplementary_Code_1.zip`: exact public code package prepared for journal upload.
- `supplementary_code_1/`: unpacked copy of Supplementary Code 1 for easier browsing and testing.
- `artwork/main_figures/`: public main-figure artwork exports.
- `artwork/supplementary_figures/`: public supplementary-figure artwork exports.
- `LICENSE.md`: license terms for public code, public summary tables, public schema/map files, and synthetic example data.
- `PUBLIC_RELEASE_MANIFEST.sha256`: checksum manifest for this public release directory.

## Run the public example

```bash
cd supplementary_code_1
python src/public_pipeline_template.py example_data/schema_example.csv
python tests/test_public_pipeline_smoke.py
```

Expected smoke-test marker:

```text
PUBLIC_SMOKE_TEST_PASS rows=10 polymer_groups=5 group_leakage.max_overlap=0
```

The public example uses synthetic data only. It checks the schema and validation code path; it does not regenerate the manuscript CatBoost metrics.

## Data boundary

This public release does not include the observation-level literature extraction table, DOI-to-record mappings, source identifiers, polymer identifiers, repeat-unit structures, row-level targets or predictions, fold assignments, raw extraction notes, trained models, local reference-manager files, or third-party article full texts.

Those materials follow the manuscript Data availability statement. Public manuscript values are provided as summary metrics in `Supplementary_Data_1.xlsx` and `supplementary_code_1/manuscript_metric_index_public.json`.

## License

The public code is released under the MIT License. Public summary tables, public schema/map files, and synthetic example data are released under CC BY 4.0. See `LICENSE.md` for the full license statement and release boundary.
