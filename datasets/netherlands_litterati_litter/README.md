# Litter counts in hexagonal grid in the Netherlands

- `litter_pois_hexagonal_grid_10sqkm_counts_w_geometries.gpkg`: Litter and POI counts in the Netherlands hexagonal grid with geometries in GeoPackage format.
- `litter_pois_hexagonal_grid_10sqkm_counts.csv`: Attribute table from the previous file in CSV format.

Each hexagon covers 10 km2.

Data dictionary: 
- `HEX10_ID`: hexagonal cell ID.
- `l_all`: Total count of Litterati litter observations.
- `l_plastic` `l_can` `l_wrapper` `l_paper` `l_metal` `l_cigarette` etc: Counts of Litterati litter observations by type.
- The `poi_` fields were collected but not used.

