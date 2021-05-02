# Litter and Google POIs for Purmerend analysis

## Data

Using a dedicated research tool that we developed (https://github.com/andrea-ballatore/google-places-api-r), we retrieved 1,420 POIs located in Purmerend from the Google Maps Places API in March 2020. This tool partitions the query area into small areas, and then generates as API queries, re-splitting the areas as needed. 
This method ensures full coverage of POIs in the target area. 

Each resulting POI is associated with a location and with multiple “types” that describe its purposes. 
In particular, the dataset includes stores (850), transit stations (255), food (246), restaurants (128), schools (22), and places of worship (19) (note that a single POI can be categorised as “food”, “meal takeaway”, and “restaurant”). 
This kind of dataset provides very high coverage and accuracy of urban POIs relevant to littering behaviour. 

Because of Google’s terms of service, the data is available in aggregated form.

The Litterati data in Purmerend includes 178,557 observations. 

## Spatial distribution

Each hexagonal cell covers 5,000 m2.

- `google_places_categories_litter.csv`: categories of POIs used in this dataset.
- `purmerend_litter_tag_counts.csv`: counts of litter tags in this dataset (> 20).
- `purmerend_litter_pois_hotspot_hexgrid5.gpkg`: litter and POI statistics with hotspot analysis in Purmerend, NL, with geometries in GeoPackage format.
- `purmerend_litter_pois_hotspot_hexgrid5_attributes.csv`: Attribute table for previous dataset.

Data dictionary:
- `freq`: number of Litterati litter observations in a hexagonal cell.
- `freq_loci`: local Moran's I.
- `freq_loci_pval`: p value for local Moran's I.
- `freq_locgistar`: local G star.
- `freq_locg_pval`: p value for local G star.
- `freq_locg_fill`: cell colour for visualisation.
- `gpoi_all`: count of all Google POIs in the cell.
- `gpoi_restaurant` etc: count of Google POIs of a specific type in the cell.

## Point pattern analysis

- ``: Co-occurrence of litter observations in Purmerend within a 100-meter radius from POIs for 25 Google POI types, including the number of POIs. 


- `purmerend_litter_pois_average_Lfunction.csv`: Average cross L-function (with z values) in range 0 to 100 meters between the most frequent 16 litter tags and 25 Google POI categories in Purmerend.

Data dictionary:
- `poi_type`: type of Google POI.
- `lit_type`: type of litter.
- `avg_L`: average cross L-function.
- `max_L`: maximum cross L-function. 	
- `avg_LZ`: Z value for average cross L-function.

