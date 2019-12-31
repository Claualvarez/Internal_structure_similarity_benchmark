## Internal_structure_similarity_benchmark

**Accuracy of the detection at the protein level**
| Benchmark set      | FiRES | ReUPred | Swelfe | CE-symm | HHrepiID | lalign | RADAR |
| :----------------- | :---: | :-----: | :----: | :-----: | :------: | :----: | :---: |
| Duplicated domains |  0.86 |  0.50   |  0.59  |  0.72   |   0.61   |  0.57  |  0.28 |
| Protein repeats    |  0.93 |  0.49   |  0.65  |  0.80   |   0.67   |  0.59  |  0.46 |

### [RepeatsDB](https://github.com/Claualvarez/Internal_structure_similarity_benchmark/blob/master/RepeatsDB/RepeatsDB_reference_units.tsv)
>Paladin L, Hirsh L, Piovesan D, et al. RepeatsDB 2.0: improved annotation,
classification , search and visualization of repeat protein structures.
Nucleic Acids Res. 2017;(D1):D308-D312. doi:10.1093/nar/gkw1136

### [MALIDUP](https://github.com/Claualvarez/Internal_structure_similarity_benchmark/blob/master/MALIDUP_set/MALIDUP_reference_units.tsv)
>Cheng H, Kim B, Grishin N V. MALIDUP: a database of manually constructed
structure alignments for duplicated domain pairs. Proteins Struct Funct Bioinforma.
2007;70(4):1162-1166. doi:10.1002/prot.21783


### The Database of no-repeats
We constructed a database of proteins without internal sequence and structure similarity from a subset of the PDB composed of 28337 non-redundant chains, as determined by BLASTClust at 30% sequence identity.
We applied three sequential filters:

1. structural symmetry filter: **SymD** Z-score < 4;
> Jha A, Flurchick KM, Bikdash M, Kc DB. Parallel-SymD : A Parallel Approach to Detect Internal Symmetry in Protein Domains. 2016;2016.
2. conserved internal sequence similarity filter: **InterPro** sequence signatures;
> Mitchell AL, Attwood TK, Babbitt PC, et al. InterPro in 2019 : improving coverage , classification and access to protein sequence annotations. Nucleic Acids Res.
3. sequence and structure evaluation using the followhing algorithms with default parameters:
   - **FiRES**
   - **HHrepID** 
   > Biegert A, Söding J. De novo identification of highly diverged protein repeats by probabilistic consistency. Bioinformatics. 2008;24(6):807-814. doi:10.1093/bioinformatics/btn039.
   - **lalign**
   > Pearson WR, Lipmant DJ. Improved tools for biological sequence comparison. Proc Natl Acad Sci USA. 1988;85(April):2444-2448.
   - **RADAR**
   > Heger A, Holm L. Rapid automatic detection and alignment of repeats in protein sequences. Proteins Struct Funct Genet. 2000;41(2):224-237.
   - **CE-symm**
   > Bliven SE, Lafita A, Rose PW, Capitani G, Prlić A, Bourne PE. Analyzing the symmetrical arrangement of structural repeats in proteins with CE-Symm. PLOS Comput Biol. 2019;15(4):e1006842. doi:10.1371/journal.pcbi.1006842.
   - **ReUPred**
   > Hirsh L, Piovesan D, Paladin L, Tosatto SCE. Identification of repetitive units in protein structures with ReUPred. Amino Acids. 2016;48(6):1391-1400. doi:10.1007/s00726-016-2187-2.
   - **Swelfe**
   > Abraham A, Rocha EPC, Pothier J. Swelfe : a detector of internal repeats in sequences and structures. Bioinformatics. 2008;24(13):1536-1537. doi:10.1093/bioinformatics/btn234.


### Other benchmark databases 

**The Dataset-non-TR** 
> Do Viet P, Roche DB, Kajava A V. TAPO: A combined method for the
identification of tandem repeats in protein structures. FEBS Lett. 2015;589(19):2611-2619. doi:10.1016/j.febslet.2015.08.025

![Structures with internal similarity in the database of no-tandem-repeats](images/No-tandem-repeats.png)

Some structures considered Asymmetric in the Internal symmetry dataset (https://doi.org/10.1371/journal.pcbi.1006842) have internal structure similarity.


![Structures with internal similarity in the domain_symm benchmark](images/Dom_symm_bench.jpg)

