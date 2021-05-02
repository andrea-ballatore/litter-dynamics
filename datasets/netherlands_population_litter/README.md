# Litterati litter data and population, Netherlands

Population data from Dutch Census (2017).

## Provinces

- `litter_vs_population_provinces_attributes_geom.gpkg`: Litter counts vs resident population by province in the Netherlands in GeoPackage format.
- `litter_vs_population_provinces_attributes.csv`: Attribute table from the previous file in CSV format.

Each row is a province with litter and population statistics.

Data dictionary:
- `Provincienaam`: province name.
- `population`: resident population.
- `litter_all`: litter observation count.
- `litter1kppl_iqr`: interquartile range.
- `litter_sd`: standard deviation.
- `n_gementee`: number of municipalities.
- `popmil`: population in millions.
- `popthou`: population in thousands.
- `litter_1kppl`: litter per 1,000 people.
- `litter_1kppl_z`: Z value.

## Municipalities

- `litter_vs_population_municipalities_attributes_geom.gpkg`: Litter counts vs resident population by gementee (municipalities) in the Netherlands in GeoPackage format.
- `litter_vs_population_municipalities_attributes.csv`: Attribute table from the previous file in CSV format.
- `correlations_by_municipality.csv`: Correlations between litter and socio-economic variables.

Each row is a municipality with litter and population statistics.

Data dictionary: 
- `GM_CODE`: municipality code.
- `GM_NAAM`: municipality name.
- `AANT_INW`: total resident population.
- `ppl_sqkm`: population density per km2.
- `l_all`: total count of Litterati litter observations.
- `l_plastic` `l_can` `l_wrapper` `l_paper` `l_metal` `l_cigarette` etc: counts of Litterati litter observations by type.
- `l1k_all`: litter observations by 1,000 people.
- `l1k_plastic` etc: litter observations by 1,000 people by litter type.