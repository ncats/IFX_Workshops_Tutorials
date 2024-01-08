# [RaMP - Relational database of Metabolomic Pathways](https://rampdb.nih.gov/)

## Description
RaMP-DB is a publicly available relational database that integrates multiple sources of biological, structural/chemical, disease, ontology and reaction annotations for analytes (metabolites, genes, proteins) from multiple resources including HMDB, KEGG, Reactome, WikiPathways, LIPIDMAPS, ChEBI, and Rhea.  The resource was initially created to:
1) enhance the ability to interpret metabolomic and multi-omic data using standardized annotations on analytes;
2) fill the gap in the availability of benchmark annotation database that was consistently used to compare pathway enrichment methods.

Today, RaMP-DB includes 254,860 chemical structures, of which 43,338 are lipids, 15,389 genes, 53,745 pathways, 807,362 metabolic enzyme/metabolite reactions, and 699 ontologies.  Notably, curation of the source data within RaMP-DB is semi-automatic to help ensure sustainability of the resource.  The curation process involves a first automatic pass for errors in ID mappings for metabolites across resources (e.g. comparison of MW and chemical properties), followed by a second manual curation.   

The main functionalities for interacting with RaMP-DB include single and batch queries as well as chemical and biological pathway enrichement analyses. Some useful utilities include the ability to input mixed IDs for analytes (e.g. LIPIDMAPS, PubChem, HMDB, etc for metabolites and UniProt, HMDB, and Ensembl IDs for genes/proteins), the ability to globally evaluate how much is known about analytes of interest, and clustering of enriched pathways for ease of interpreting enrichment results.  The web interface is served by APIs that can also serve as endpoints for integrating RaMP-DB with other tools.  Finally, RaMP-DB users can also directly download the database as a MySQL dump or SQLite for their own mining or incorporation into other tools.        

## Workshop Vignette
Access the workshop vignette [here](https://ncats.github.io/IFX_Workshops_Tutorials/202311_AMIA_Workshop/RaMP/RaMPDB_QuickIntro.html).  The RMarkdown file used to create this "Quick Intro" vignette can be found in this folder (RaMPDB_QuickIntro.Rmd).

## RaMP-DB Access and Contact
- [R package](https://github.com/ncats/RaMP-DB/tree/sqlite) - The latest package is on the SQLite branch will be released this month!
- For the user-friendly web interface, [click here](https://rampdb.nih.gov/).
- For API access, [click here](https://rampdb.nih.gov/api).

Direct any questions through the Issues tab in GibHub or via email at [NCATSRaMP@nih.gov](mailto:NCATSRaMP@nih.gov).
