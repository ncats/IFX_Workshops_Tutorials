## Scavenger Hunt with answers <a id="scavenger hunt"></a>
1. Finding primary documentation
   1. What is the MONDO description for "asthma?"
        * A bronchial disease that is characterized by chronic inflammation and narrowing of the airways...
   2. How many Tclin targets have associations to this disease?
      * 53
   3. Which sub-class of "asthma" has the most target associations?
      * occupational asthma (10) 
2. Finding ligands for a target
   1. Find the details page for target MAPK11
      * https://pharos.ncats.nih.gov/targets/MAPK11
   2. How many active compounds are there for that target?
      * Active Ligands (42) - no approved drugs
   3. How many have a potency above greater than or equal to 8? (i.e. 1e-8 M = 10nM)
      * 18 ligands
         * click explore active ligands on the target details page
         * filter Potency to above 8.0
   4. How many are selective for that target? (how many have only one documented target activity)
        * 11 ligands in the list have only activity to only one target
        * ...however there could be activities to other targets that aren't found in ChEMBL or DrugCentral
3. Illuminating a dark target
   1. What TDL is RAD21L1?
      * Tdark
      * https://pharos.ncats.nih.gov/targets/RAD21L1
   2. How many direct disease associations does it have?
      * 0
   2. How many interacting targets does it have?
      * 111
   3. What is the most common disease associated with RAD21L1?
      * ovarian cancer (65)
   4. What is the top two diseases that are enriched in the population of interacting targets?
      * Roberts syndrome (7 targets)
      * primitive neuroectodermal tumor (48 targets)
   5. What targets have sequence similarity to Gene X? (return to target details page - find the sequence)
        * 2 targets - RAD21, REC8
4. Disease Lists
   1. How many diseases are in Pharos
      * 13,953
   2. How many are annotated to be Rare Diseases, based on GARD?
      * 2,967
   3. Of those rare diseases, how many have an associated target that has an approved drug?
      * (hint) - Tclin targets have an activity to an approved drug
      * 827
5. Investigating a new chemical compound
   1. Example smiles - CC1CC(O)(CCN1CCCC(=O)C1=CC=C(F)C=C1)C1=CC=C(Cl)C=C1
   2. How many ligands in Pharos have some structural similarity?
      * 1,810
   3. How many ligands hav 0.8 or greater similarity
      * 66
   4. What target has activity to the most ligands in that list?
      * D2 Dopamine Receptor
6. Using UpSet Plots
   5. How many targets were on the Original IDG List?
      * 416
   6. How many targets are on the current IDG List (2022 list)?
      * 313
   7. How many were on the original list, but are no longer on the current IDG List?
      * 104
      * https://pharos.ncats.nih.gov/analyze/targets?facet=NIH%2BTarget%2BLists!InGroup:IDG%2520Original%2520(2017)OutGroup:IDG%2520Refined%2520(2022)
