Start with trich.Rmd to read our draft manuscript. See trich-prep.Rmd for the bulk of the code used in generating this manuscript.

# File List:

- **trich.Rmd** : main manuscript file

- **plantarum.json** : bibliography (exported from Zotero, only necessary to
  regenerate citations and literature cited when compiling manuscript)

- **trich-prep.Rmd** : The bulk of the code used in the analysis. Loaded from
  trich.Rmd to regenerate the figures and tables there.

- **american-journal-of-botany.csl** : formatting specification for AJB
  articles. I don't recall where this came from; only necessary to format
  references when compiling manuscript.

- **data/ssr_raw.csv** : raw microsatellite data. See trich-prep.Rmd (Loading
  Data) for code to load and translate this to a genind object

- **data/survey-pops.csv** : coordinates of sampled populations

- **data/background_points.csv** : 10,000 random sampled from the study extent,
  used in the Maxent modeling. You could easily recreate a comparable data
  set within R, but I didn't know that when I generated this file in QGIS.

- **data/eval.opt.2020-06-24.Rda** : the output of the Maxent modeling, saved
  as a binary R Data object. Load into R with the load() function, so you
  don't need to repeat the lengthy Maxent analysis.

- **data/trich-gbif.csv** : GBIF records used in the Maxent analysis

- **data/trich_soil.csv** : Soil analysis for each sampled population

- **data/maps** : Maps (shapefiles and rasters) used in the Maxent analysis,
  and for some of the manuscript plots


