# Daycare analysis

This repo contains data and python scripts for working with daycare violation data outside of data warehouse. The notebooks run in a default conda environment.

### Raw data

The `csv/dfps-2018-02-01/` directory contains the raw files DFPS tables for
- [non-compliance](https://data.texas.gov/Social-Services/DFPS-CCL-Non-Compliance-Data/tqgd-mf4x)
- [operations](https://data.texas.gov/Social-Services/DFPS-CCL-Daycare-and-Residential-Operations-Data/bc5r-88dy)
- [standards](https://data.texas.gov/Social-Services/DFPS-CCL-Sections-and-Standards-Evaluated-Data/ywgb-2ig8/)
- [assessment](https://data.texas.gov/Social-Services/DFPS-CCL-Inspection-Investigation-Assessment-Data/m5q4-3y3d)

as they were on Feb. 1, 2018. These files are used for analysis.

### Filtering possible injuries

The notebook at `notebooks/data_warehouse_export.ipynb` filters the DFPS data for review of possible injuries. The resulting dataset is imported into the [daycare-injuries](https://github.com/statesman/data-warehouse/tree/master/daycare_injuries) data warehouse app with a management command.
