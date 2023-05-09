# RML RULES FOR RDF Production

This repository includes some CSV datasets we are using in the WHOW project in order to transform them in RDF graphs composign the WHOW knowledge graph.
In particular, the transformations provided in this repository are:

1) Python scripts to carry out data cleansing activities;
2) RML (RDF Mapping Language) rules for transforming typically tabular data into RDF-based datasets forming the WHOW knowledge graph.

In particular, within the RML-RULES directory there are different directories; each directory is related to produced RDF datasets and includes the original CSV files and other supporting CSV files, the RML Rules (RDF/turtle file), and in some cases the output in RDF produced. The structure is the following:

1) **chemical sustance mapping**: this directory includes the RML rules necessary to create the [WHOW controlled vocabulary on chemical sustances](https://w3id.org/whow/controlled-vocabulary/chemical-substances) that is linked to the related concepts available in Wikidata. We used two types of CSV files: one coming from the monitoring of the quality of water bodies of different types (e.g., rivers, lakes), and one used in the pesticides domain. This dataset mainly serves the WHOW use case 2.

2) **diseases**: this directory includes the RML rules necessary to create the [WHOW controlled vocabulary on (infectious) diseases](https://w3id.org/whow/controlled-vocabulary/diseases) that is linked to snomed ontology. We used the open dataset on the monitoring of the infectious diseases rates of Lombardy region to create the RDF dataset. This dataset mainly serves the WHOW use case 2.

3) **hydrography**: this directory includes two additional directories with the RML rules necessary to create the list of lakes and rivers of the lombardy region. The RDF datasets, linked to Wikidata and DBpedia, have been obtained by applying the RML rules to datasets on the monitoring of the quality of rivers and lakes. These datasets mainly serve the WHOW use case 2.

4) **infection disease monitoring**: this directory includes the RML rules necessary to create the RDF graph of the distribution of the diseases by age and sex in the Lombardy region. The original CSV open dataset is included in this directory. This dataset mainly serves the WHOW use case 2.

5) **observable properties mapping**: this directory includes the RML rules necessary to create a specific datasets on the observable properties, defined in the Observation-Measure pattern and used for the monitoring of the quality of water for rivers, lakes and groundwaters. This dataset mainly serves the WHOW use case 2.

6) **ostreopsis mapping**: this directory includes the RML rules and the original CSV files to create the dataset on the monitoring of the presence of the ostreopsis ovata algae in marine waters. These datasets, available for years 2020 and 2021, support the WHOW use case 1.

7) **water monitoring groundwaters**: this directory includes the RML rules and the original CSV files to create the dataset on the monitoring of the quality of groundwaters of the Lombardy region. This dataset serves the WHOW use case 2.

8) **water monitoring lakes**: this directory includes the RML rules and the original CSV files to create the dataset on the monitoring of the quality of lakes of the Lombardy region. This dataset serves the WHOW use case 2.

9) **water monitoring rivers**: this directory includes the RML rules and the original CSV files to create the dataset on the monitoring of the quality of rivers of the Lombardy region. This dataset serves the WHOW use case 2.

10) **weather monitoring**: this directory includes the RML rules and the original CSV files to create specific datasets, currently related to one month only of 2019, on the meteorological conditions of the Lombardy region. These datasets serve the WHOW use case 3, together with other datasets on the soil consumption indicators and the intervention on the territory published by ISPRA, queryable through ISPRA's SPARQL endpoint and not available on this repository.
