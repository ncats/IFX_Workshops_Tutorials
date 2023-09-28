# Pharos: Illuminating the Druggable Genome

[Pharos](https://pharos.nih.gov/) is the flagship web interface for the 
Illuminating Druggable Genome (IDG) Consortium, an NIH Common Fund 
project. Pharos integrates cutting-edge informatics tools and serves 
as your portal to access valuable insights and resources about 
understudied protein targets. 

This workshop will help you explore, analyze, and download data via
the web platform, as well as programmatically through the API.

## Table of Contents

1. [Introduction to Pharos](#introduction-to-pharos)
2. [Tools for your toolbox](#tools-for-your-toolbox)
   1. [Finding specific targets, diseases, or ligands](#finding-pages)
   2. [Reviewing primary documentation](#review-primary)
   3. [List pages](#list-pages)
   4. [Expanding the search for data](#expanding-the-search)
   5. [UpSet Plots](#upset-plots)
   6. [Calculating Enrichment](#calculating-enrichment)
   7. [Downloading data](#downloading-data)
3. [Challenges](#challenges)
4. [Contact Us](#contact-us)

## Introduction to Pharos <a id="introduction-to-pharos"></a>

Pharos is a cutting-edge web tool designed to streamline your research and data analysis tasks.
It offers a wide range of features to help you explore, visualize, and analyze your 
datasets efficiently.


## Tools for your toolbox <a id="tools-for-your-toolbox"></a>
###1. Finding specific targets, diseases, or ligands <a id="finding-pages"></a>
TODO
###2. Reviewing primary documentation <a id="review-primary"></a>
TODO
###3. List pages <a id="list-pages"></a>
TODO
###4. Expanding the search for data <a id="expanding-the-search"></a>
TODO
###5. UpSet Plots <a id="upset-plots"></a>
TODO
###6. Calculating Enrichment <a id="calculating-enrichment"></a>
TODO
###7. Downloading data <a id="downloading-data"></a>
TODO

## Challenges <a id="challenges"></a>
1. Finding primary documentation
   1. What is the MONDO description for ""
   2. How many Tclin targets have associations to this disease
   3. Which sub-class of "" has the most target associations
2. Finding ligands for a target
   1. Find the details page for target X
   2. How many active compounds are there for that target (both approved and unapproved)?
   3. How many have a potency above X?
   4. How many seem selective for that target? (how many have 2 or fewer targets with activities)
3. Illuminating dark targets
   1. How many direct disease associations does Gene X have?
   2. How many interacting targets does Gene X have?
   3. What diseases are associated with the interacting targets
   4. What is the top disease that is enriched in the population of interacting targets?
   5. What targets have sequence similarity to Gene X?
   6. What diseases are those targets associated with?
4. Disease Lists
    1. How many are annotated to be Rare Diseases, based on GARD?
    2. Of those rare diseases, how many have an associated target that has an approved drug?
       1. (hint) - Tclin targets have an activity to an approved drug
5. Investigating target-disease associations
    1. What GO functions are annotated on those targets
    2. What GO functions are enriched in this target list
6. Investigating a new chemical compound
   1. What ligands in Pharos have some structural similarity?
   2. Filter the list to only ligands that have 0.8 or greater similarity.
   3. What targets have activity to those ligands?
   4. How many ligands in th
7. Using UpSet Plots
   5. How many targets were on the Original IDG List?
   6. How many targets are on the current IDG List?
   7. How many were on the original list, but are no longer on the current IDG List?
    
## Contact Us <a id="contact-us"></a>

We're here to help! If you have any questions, feedback, or need assistance, please feel free to reach out to our 
team at [pharos@mail.nih.gov](mailto:pharos@mail.nih.gov).
