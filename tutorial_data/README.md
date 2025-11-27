# The data

* `argo_bgc_global_surface_*`: All the mean surface measurements from Bio-Argo for March 2024 to Nov 23, 2025. CHLA is depth < 20m, while BBP700 is depth < 10m.
* `*_argo_rrs_all` and `*_argo_rrs`: The matchups with PACE Rrs. all includes NaNs in Rrs while the other file has NaN rows removed. NaNs are places where clouds or glint or something prevented a Rrs value. The `pace_Rrs_lat`/`pace_Rrs_lon` columns are the matched (nearest) values from the PACE Rrs (level 3) data while the `LATITUDE`/`LONGITUDE` columns are what is in the Bio-Argo data.
* `*_argo_rrs_chl_all` and `*_argo_rrs_chl`: The matchups with PACE Rrs and CHL. `all` includes NaNs in Rrs while the other file has NaN Rrs rows removed. NaNs are places where clouds or glint or something prevented a Rrs value (and CHL since it is computed from that). The `pace_Rrs_lat`/`pace_Rrs_lon` columns are the matched (nearest) values from the PACE Rrs (level 3) data while the `LATITUDE`/`LONGITUDE` columns are what is in the Bio-Argo data.

# Notebooks

* `argopy.ipynb`: created `argo_bgc_global_surface_*`
* `argopy-matchups.ipynb`: created `*_argo_rrs_all` and `*_argo_rrs`.