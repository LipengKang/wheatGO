# wheatGO
wheatGO is scripts based on clusterProfiler or Ontologizer for wheat function analysis.

The version 1.1 contains 3 go annotation resource (Ensembl, agroiGO and GOMAP) and 2 kinds of enrichment algorithms (Term-For-Term and Parent-child). In ALL, it can hold on 6 main recombinations of GO enrichment.

It is a first step for GO analysis. Both clusterProfiler and Ontologizer is recommended to do cross-validation. Furthermore, highly cited websites, AgriGo(Tian, 2017) or Plant Regulomics(Ran, 2019), are also highly recommended.

## PREREQUISITES

**Java:**  Runtime >= 52.0 (Version >= 8)

**R:** (Version >=  3.6.3)

**R package:** clusterProfiler, optparse


## INSTALLATION

Download the latest version 'wheatGO`  in Release.



## Usage
./wheatGO-v1.1-Ontologizer

./wheatGO-v1.1-clusterProfiler

### Recomended usage
**example1:** ./wheatGO-v1.1-Ontologizer -g test/T1.txt -m GOMAP -c Parent-Child-Intersection -p Benjamini-Hochberg -r 100

Sets of T1 genes were assessed for GOMAP using ontology term enrichment with the Parent-Child-Intersection method implemented in the Ontologizer software.


**exmaple2:** ./wheatGO-v1.1-clusterProfiler [options] -g test/T1.txt -m GOMAP -a directAnno

Sets of T1 genes were assessed for GOMAP using ontology term enrichment with the enricher method implemented in the clusterProfiler software. It is a Term-For-Term method.

**For further information, please see README in release**

## Reference
Tian Tian, Yue Liu, Hengyu Yan, Qi You, Xin Yi, Zhou Du, Wenying Xu, Zhen Su; agriGO v2.0: a GO analysis toolkit for the agricultural community, 2017 update. Nucleic Acids Res 2017 gkx382. doi: 10.1093/nar/gkx382

Xiaojuan Ran#, Fei Zhao#, Yuejun Wang#, Jian Liu, Yili Zhuang, Luhuan Ye, Meifang Qi, Jingfei Cheng and Yijing Zhang*. (2019), Plant Regulomics: A Data-driven Interface for Retrieving Upstream Regulators from Plant Multi-omics Data[J]. The Plant Journal. doi: 10.1111/tpj.14526
