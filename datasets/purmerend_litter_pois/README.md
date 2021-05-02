# Data for Purmerend analysis

## Google's Points of Interest

Using a dedicated research tool that we developed (https://github.com/andrea-ballatore/google-places-api-r), we retrieved 1,420 POIs located in Purmerend from the Google Maps Places API in March 2020. This tool partitions the query area into small areas, and then generates as API queries, re-splitting the areas as needed. 
This method ensures full coverage of POIs in the target area. 

Each resulting POI is associated with a location and with multiple “types” that describe its purposes. 
In particular, the dataset includes stores (850), transit stations (255), food (246), restaurants (128), schools (22), and places of worship (19) (note that a single POI can be categorised as “food”, “meal takeaway”, and “restaurant”). 
This kind of dataset provides very high coverage and accuracy of urban POIs relevant to littering behaviour. 

Because of Google’s terms of service, the data is available in aggregated form.

Every hexagonal cell covers 5,000 m2.

- `puremerend_pois_hexagonal_grid_5.gpkg`: POI statistics for hexagonal cells in Purmerend, NL, with geometries in GeoPackage format.
- `puremerend_pois_hexagonal_grid_5_attributes.csv`: Attribute table for previous dataset.
- `google_places_categories_litter.csv`: categories of POIs selected in this dataset.

Data dictionary:
- `gpoi_all`: count of all Google POIs in the cell.
- `gpoi_restaurant` etc: count of Google POIs of a specific type in the cell.

## Hotspot analysis

Every hexagonal cell covers 5,000 m2.

- `puremerend_litter_hexagonal_grid_5_hotspot.gpkg`: 
- `puremerend_litter_hexagonal_grid_5_hotspot_attributes.csv`: 

Data dictionary:
- `freq`: frequency of litter observations.
- `freq_loci`: local Moran's I.
- `freq_loci_pval`: p value for local Moran's I.
- `freq_locgistar`: local G star.
- `freq_locg_pval`: p value for local G star.
- `freq_locg_fill`: cell colour for visualisation.
- Other columns are not used.