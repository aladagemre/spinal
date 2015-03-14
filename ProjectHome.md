## Overview ##
We provide the SPINAL  algorithm for the problem of globally aligning a pair of PPI networks. Our algorithm proceeds in two phases. In the first coarse-grained alignment phase we construct all pairwise initial similarity scores based on pairwise local neighborhood matchings. Employing the produced similarity scores, the fine-grained alignment phase produces the final one-to-one mapping by iteratively growing a locally improved solution subset. Both phases make use of the construction of "neighborhood bipartite graphs" and the "contributors" as a common primitive.  We assess the performance of our algorithm on the PPI networks of yeast, fly, human, and worm. We show that based on the accuracy measures employed in relevant work, our method outperforms the state-of-the-art algorithms. Furthermore our algorithm does not suffer from scalability issues, as such accurate results are achieved in reasonable running times as compared to the benchmark algorithms.

## Supplementary Document ##
Supplementary descriptions and evaluations are provided in the Supplementary Document, which can be accessed through the Downloads.

## Downloads ##
The complete SPINAL package including open source code in C++ LEDA, executable binary(compiled under Linux 64 bit system), useful scripts, necessary data files, and output results can be found under Downloads.

## Contacts ##
  * [Cesim Erten](http://hacivat.khas.edu.tr/~cesim), Computer Engineering, Kadir Has University, Istanbul, Turkey
  * [Ahmet Emre Aladağ](http://www.emrealadag.com), Computer Engineering, Bogazici University, Istanbul, Turkey

## Requirements ##
Binary executable is compiled on a 64 bit Linux system. Compilation from source code requires [LEDA Professional Library 5.1](http://www.algorithmic-solutions.com). Codes are licensed under GPL v3 License but the binaries are under Academic Free license due to LEDA license restrictions.

## Sample Alignment ##
SPINAL output alignment network of the H.Sapiens-S.Cerevisiae data. Only the maximum connected component of the alignment network induced by alignment pairs sharing at least one GO category overlap are shown. There are 487 nodes (alignment pairs) in this induced subgraph. Blue nodes are those with one GO annotation overlap, green nodes are those with two overlaps, and pink nodes are those with at least three overlaps. The top ten maximum degree alignment nodes (those with largest number of conserved interactions) are below.

1: SMAD2 | YDR388W,
2: EP300 | YMR308C,
3: CREBBP | YOR294W,
4: PTK2 | YBR109C,
5: CAV1 | YDR414C,
6: ATXN1 | YKR048C,
7: AR | YPL022W,
8: ESR1 | YEL037C,
9: YWHAE | YLR150W,
10: MYC | YAL005C
![http://spinal.googlecode.com/svn/samplealign/hsapi-scere-spinalmatch-alignmentgosubgraphmaxcompdrawing7.png](http://spinal.googlecode.com/svn/samplealign/hsapi-scere-spinalmatch-alignmentgosubgraphmaxcompdrawing7.png)