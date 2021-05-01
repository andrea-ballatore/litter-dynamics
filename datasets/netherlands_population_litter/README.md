# Litter vs population at the gementee level (municipalities), Netherlands

- `litter_vs_population_gementee_municipalities_netherlands_attributes_geom.gpkg`: Litter counts vs resident population by gementee (municipalities) in the Netherlands in GeoPackage format.
- `litter_vs_population_gementee_municipalities_netherlands_attributes`: Attribute table from the previous file in CSV format.

Each hexagon covers 10 km2.

fid			WATER	OAD	STED	AANT_INW	AANT_MAN	AANT_VROUW	P_00_14_JR	P_15_24_JR	P_25_44_JR	P_45_64_JR	P_65_EO_JR	P_ONGEHUWD	P_GEHUWD	P_GESCHEID	P_VERWEDUW	BEV_DICHTH	AANTAL_HH	P_EENP_HH	P_HH_Z_K	P_HH_M_K	GEM_HH_GR	P_WEST_AL	P_N_W_AL	P_MAROKKO	P_ANT_ARU	P_SURINAM	P_TURKIJE	P_OVER_NW	OPP_TOT	OPP_LAND	OPP_WATER	Shape_Leng	Shape_Area	income2017	l_all	l_plastic	l_can	l_wrapper	l_paper	l_metal	l_cigarette	l_bottle	l_candy	l_beer	l_bag	l_piece	l_energydrink	l_firework	l_redbull	l1k_all	l1k_plastic	l1k_can	l1k_wrapper	l1k_paper	l1k_metal	l1k_cigarette	l1k_bottle	l1k_candy	l1k_beer	l1k_bag	l1k_piece	l1k_energydrink	l1k_firework	l1k_redbull	Provincienaam	OBJECTID	litt_100kppl	litt_1kppl	litt_1k_log_ppl	unit_area	ppl_sqkm

Data dictionary: 
- `GM_CODE`: municipality code.
- `GM_NAAM`: municipality name.
- `AANT_INW`: total resident population.
- `l_all`: total count of Litterati litter observations.
- `l_plastic` `l_can` `l_wrapper` `l_paper` `l_metal` `l_cigarette` etc: counts of Litterati litter observations by type.
- `l1k_all`: litter observations by 1,000 people.
- `l1k_plastic` etc: litter observations by 1,000 people by litter type.
- The other fields were collected but not used.
