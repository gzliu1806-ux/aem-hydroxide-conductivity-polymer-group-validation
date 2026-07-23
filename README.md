# Polymer-group validation of AEM hydroxide-conductivity models

This repository accompanies the manuscript *Polymer-group validation of hydroxide-conductivity models for anion exchange membranes: data leakage, descriptor interpretation, and source heterogeneity*.

It provides public summary tables, field definitions, fitted response coordinates, and a synthetic example of polymer-group validation. The example is designed to show the validation interface and data boundaries; it does not regenerate manuscript metrics from the non-public observation-level literature table.

## Release contents

- `Supplementary_Data_1.xlsx`: editable Tables S1-S15.
- `Supplementary_Code_1.zip`: archive of the runnable public example.
- `supplementary_code_1/`: expanded copy of Supplementary Code 1.
- `extended_aem_response_atlas/`: 48 fitted AEM response profiles for diagnostic review; this extension is not part of the formal Supporting Information.
- `PUBLIC_RELEASE_MANIFEST.sha256`: checksums for the files in this release.

## Quick check

```bash
cd supplementary_code_1
python tests/test_public_pipeline_smoke.py
```

The smoke test checks a 10-row synthetic dataset containing five polymer groups. The grouped split must report zero polymer overlap. Reported CatBoost metrics are indexed in `supplementary_code_1/manuscript_metric_index_public.json` and tabulated in `Supplementary_Data_1.xlsx`.

## Data boundary

The repository does not contain the observation-level literature extraction table, source or polymer identifiers, DOI-to-record mappings, article-level extraction notes, fold assignments, trained models, or row-level targets and predictions. Access to verification materials follows the manuscript Data availability statement. Third-party article full texts are not redistributed.

## License

Code is released under the MIT License. Public summary tables and synthetic example data are released under CC BY 4.0. See `LICENSE.md` for scope and exclusions.
