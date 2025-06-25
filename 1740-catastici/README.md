# 1740 Catastici

# Files
* `1740_catastici_version20250625.geojson`: transcription of the Catastici with data relating to the disambiguation of people and institution or other kind of named entities. Information on how such data was produced can be found in `index/README.md`.
* `index`: scripts and documentation on how people disambiguation and named entity recognition was performed to obtain the aforementionned file by Carlo Musso. Left here as documentation/inspiration.


# Data Fields

## From the transcription

-  `owner_name`: Name of the owner (raw).
-  `ten_name`: Name of the tenant (raw).
-  `function`: Function of the parcel.
-  `an_rendi`: Rent paid.
-  `place`: Indication of the place where the parcel is located, can contain information about the place's function or a unique toponym related to this place.
- `quantity_income`: In rare cases, rent is not collected in cash, but in other forms. This field is the amount.
- `quality_income`: In rare cases, rent is not collected in cash, but in other forms. This field is the nature.
- `sestiere`: District name.
- `geometry`: Position of the point.

  
## Operational

- `uid`: Unique identifier of the entry drawn using a pencil. The sequence of number was restarted at each parish. It is a combination of the parish (three-letter code) and the number within the parish. `CNC-0001` is e.g. the entry #0001 for the San Cancian parish.
- `author`: author of the transcription.
- `tif_path_img`: Path to the TIF scan of the archival document.

## Standardized / Additonial fields

- `owner_code`: Code of owner type
- `owner_count`: number of owners (type `str` as some entries have an unspecified number >1 and are listed as 1+)
- `id_napo`: Whenever found, the corresponding parcel in the Sommarioni 1808.
- `PP_Function_TOP`: Aggregated category of the function.
- `PP_Function_MID`: Category of the function.
- `PP_Function_PROPERTY`: Type of ownership (when specified).
- `PP_Function_GEOMETRY`: Type of geometry (when specified).
- `PP_Bottega_STD`: Standardisation of shop nature.
- `PP_Bottega_COUNT`: Number of shops.
- `PP_Bottega_TRAD`: Translation of the shop nature.
- `PP_Bottega_METACATEGORY`: Aggregated category of shops.
- `PP_Owner_Title`: Owner title.
- `PP_Owner_Entity`: Owner entity.
- `PP_Owner_FirstName`: Owner first name.
- `PP_Owner_LastName`: Owner last name.
- `PP_Owner_Notes`: Notes on the owner field.
