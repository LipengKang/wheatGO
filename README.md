# wheatGO
A set of command line tools for GO enrichment of wheat.


## PREREQUISITES

**Java:**  Runtime >= 52.0 (Version >= 8)

**R:** (Version >=  3.6.3)

**R package:** clusterProfiler, optparse


## INSTALLATION

Download the latest version 'wheatGO`  in Release.

## Usage
./wheatGO-v1.0-Ontologizer
./wheatGO-v1.0-clusterProfiler

### Recomended usage
**example1:** ./wheatGO-v1.0-Ontologizer -g test/T1.txt -m GOMAP -c Parent-Child-Intersection -p Benjamini-Hochberg -r 100

Sets of T1 genes were assessed for GOMAP using ontology term enrichment with the Parent-Child-Intersection method implemented in the Ontologizer software.


**exmaple2:** ./wheatGO-v1.0-clusterProfiler [options] -g test/T1.txt -m GOMAP -a directAnno

Sets of T1 genes were assessed for GOMAP using ontology term enrichment with the enricher method implemented in the clusterProfiler software. It is a Term-For-Term method.
