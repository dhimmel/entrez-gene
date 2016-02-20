# Creating user-friendly Entrez Gene datasets for humans

[![DOI: 10.5281/zenodo.45524](https://zenodo.org/badge/doi/10.5281/zenodo.45524.svg)](http://dx.doi.org/10.5281/zenodo.45524 "Zenodo deposition of this repository")

Entrez Gene is the NCBI database of gene-specific information. It provides "tracked, unique identifiers for genes" and reports "information associated with those identifiers for unrestricted public use [[source](https://doi.org/10.1093/nar/gki031 "Entrez Gene Publication: gene-centered information at NCBI")]." We [use Entrez Gene](https://doi.org/10.15363/thinklab.d34 "Thinklab discussion: Using Entrez Gene as our gene vocabulary") as the primary gene vocabulary for our drug repuposing research.

This repository creates user-friendly datasets from Entrez Gene. We currently focus on human genes only.

The python notebook [`process.ipynb`](process.ipynb) executes the analysis. Files downloaded from external locations are stored in [`download`](download). The following created datasets reside in [`data`](data):

+ [`genes-human.tsv`](data/genes-human.tsv): human genes with a select set of fields storing additional attributes
+ [`symbols-human.tsv`](data/symbols-human.tsv): a table of GeneID, symbol, and symbol type (synonym or primary)
+ [`symbols-human.json`](data/symbols-human.json): a Symbol–GeneID mapping of primary symbols only
+ [`synonyms-human.json`](data/synonyms-human.json): a Symbol–GeneIDs mapping for synonyms
+ [`symbol-map.json`](data/symbol-map.json): a Symbol–GeneID mapping with approved symbols and unambiguous synonyms
+ [`xrefs-human.tsv`](data/xrefs-human.tsv): mappings to external resources
