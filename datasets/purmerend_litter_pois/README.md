# TODO

puremerend_litter_pois_hexagonal_grid_5.geojson

Using a dedicated research tool that we developed (https://github.com/andrea-ballatore/google-places-api-r), we retrieved 1,420 POIs located in Purmerend from the Google Maps Places API in March 2020. This tool partitions the query area into small areas, and then generates as API queries, re-splitting the areas as needed. 
This method ensures full coverage of POIs in the target area. 

Each resulting POI is associated with a location and with multiple “types” that describe its purposes. 
In particular, the dataset includes stores (850), transit stations (255), food (246), restaurants (128), schools (22), and places of worship (19) (note that a single POI can be categorised as “food”, “meal takeaway”, and “restaurant”). 
This kind of dataset provides very high coverage and accuracy of urban POIs relevant to littering behaviour. 

Because of Google’s terms of service, this data cannot be made available for replicability.