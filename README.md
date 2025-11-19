# Geospatial Analysis of Petroleum Spills in New York State

## About

This repository contains a geospatial analysis examining the distribution of petroleum spill incidents across New York State counties during January-October 2023. The analysis combines environmental incident reporting data with Census Bureau geographic boundaries to create choropleth visualizations and identify spatial patterns in petroleum spills.

The project demonstrates:
- Integration of tabular incident data with geospatial boundary files
- Data cleaning and standardization techniques for multi-source datasets
- Geospatial data wrangling using `geopandas`
- Professional cartographic visualization with `matplotlib`
- Reproducible data science workflow practices

This work was completed as part of EDS 220 - Working with Environmental Datasets in the UCSB Master of Environmental Data Science program.

## Repository Structure

```
eds220-hwk3/
│
├── hwk3-task1-spills.ipynb    # Main analysis notebook
├── data/                       # Data directory (not tracked in git)
│   ├── Spill_Incidents_20251102.csv
│   └── tl_2023_us_county.zip
├── tests/                      # Grading test files
├── README.md                   # This file
├── LICENSE                     # Repository license
└── .gitignore                  # Git ignore file
```

## Data

### Data Sources

**NYS DEC Spill Incidents Dataset**
Incident reports of petroleum and hazardous material spills in New York State, maintained by the New York State Department of Environmental Conservation and published through the Open Data NY portal.

**US Census TIGER/Line Shapefiles**
County boundary polygons for the United States from the U.S. Census Bureau, providing geographic reference data for spatial analysis.

### Data Access

The datasets used in this analysis are **not included** in this repository due to file size constraints. To reproduce this analysis:

1. **Spill Incidents Data**: Download from [Open Data NY - Spill Incidents](https://data.ny.gov/Energy-Environment/Spill-Incidents/u44d-k5fk)
   - Save as: `data/Spill_Incidents_20251102.csv`

2. **County Boundaries**: Download from [Census Bureau TIGER/Line Shapefiles](https://www.census.gov/geographies/mapping-files/time-series/geo/tiger-line-file.2022.html#list-tab-790442341)
   - Select "2023" year and "Counties (and equivalent)" layer type
   - Save the zip file as: `data/tl_2023_us_county.zip`

3. Create a `data/` directory in the repository root if it doesn't exist
4. Place both files in the `data/` directory

The `data/` directory is excluded from version control via `.gitignore` to prevent committing large data files.

## Requirements

This analysis requires Python 3.x with the following packages:
- `pandas` - Tabular data manipulation
- `geopandas` - Geospatial data operations
- `matplotlib` - Visualization
- `numpy` - Numerical operations

## References

New York State Department of Environmental Conservation. (2025). *Spill incidents* [Data file]. Open Data NY. Retrieved November 2, 2025, from https://data.ny.gov/Energy-Environment/Spill-Incidents/u44d-k5fk

U.S. Census Bureau, Geography Division. (2023). *TIGER/Line shapefiles: 2023 counties (and equivalent)* [Data file]. Retrieved November 2, 2025, from https://www.census.gov/geographies/mapping-files/time-series/geo/tiger-line-file.2022.html

Wingate, C. (2024). *EDS 220: Working with environmental datasets* [Course materials]. Master of Environmental Data Science, Bren School of Environmental Science & Management, University of California, Santa Barbara. https://meds-eds-220.github.io/MEDS-eds-220-course/

## License

This project is licensed under the terms included in the LICENSE file.

---

*This project is part of the curriculum for the Master of Environmental Data Science program at the Bren School of Environmental Science & Management, UC Santa Barbara.*
