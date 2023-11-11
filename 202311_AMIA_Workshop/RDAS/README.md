#[RDAS - Rare Disease Alert System](https://rdas.ncats.nih.gov/)
https://rdas.ncats.nih.gov/
##1. description
Rare Disease Alert System (RDAS) is an effort to aggregate and harmonize rare disease data from a multitude of sources and present it in a concise format. Publication, Funding, Trial and Epidemiological data are mapped and annotated to a common disease ontology. Users are also able to subscribe to receive email alerts when there is updated information available about a disease of interest. 
##2. use cases/walkthroughs

1. [Finding specific diseases](#finding-pages)
2. [List pages](#list-pages)
3. [Filtering diseases](#filtering)
4. [Downloading data](#downloading-data)
5. [Programmatic access](#apis)
6. [Epidemiology API](#epi)
7. [Neo4j](#neo4j)
8. [GraphQL](#graphql)


##3. sample queries
get diseases associated with a gene
```aidl
MATCH (n:GARD)-[]-(g:Gene {GeneSymbol: "HTT"}) 
RETURN n.GardId, n.GardName, collect(g.GeneSymbol) LIMIT 25
```
get diseases associated with a gene, and other related genes
```aidl
MATCH (n:GARD)-[]-(g:Gene) with collect (g.GeneSymbol) as genes, n
WHERE "HTT" IN genes
RETURN n.GardId, n.GardName, genes
LIMIT 25
```
get application ids for projects involving those diseases
```aidl
MATCH p=(n:GARD)-[r:RESEARCHED_BY]-(pr:Project) 
WHERE n.GardId IN ["GARD:0017965", "GARD:0010510","GARD:0006677"] 
RETURN n.GardId, collect(pr.application_id)
```
##4.Sample inputs
get diseases associated with a gene
```aidl
query GardsfromGene {
  gards(where: { associatedWithGeneGenes_SOME: { GeneSymbol: "HTT" } }) {
    GardName
    GardId
  }
}
```
get diseases associated with a gene, and other related genes
```aidl
query Genes {
  genes(where: { GeneSymbol: "HTT" }) {
    GeneSymbol
    GeneTitle
    gardSassociatedWithGene {
      GardId
      GardName
    }
  }
}
```
get application ids for projects involving those diseases
```aidl
query Projects {
  projects(
    where: {
      gardsresearchedBy_SOME: {
        GardId_IN: ["GARD:0017965", "GARD:0010510", "GARD:0006677"]
      }
    }
  ) {
    application_id
  }
}
```

##5. Contact us 
ncatsrdas@mail.nih.gov
