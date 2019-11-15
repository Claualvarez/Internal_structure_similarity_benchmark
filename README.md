# Internal_structure_similarity_benchmark

We constructed a database of proteins without internal sequence and structure similarity. 
To this end, we used three sequential filters on a subset of the PDB composed of 28337 non-redundant chains, as determined by BLASTClust
at 30% sequence identity:

1) structural symmetry filter: SymD [1] Z-score < 4;
2) conserved internal sequence similarity filter: InterPro sequence signatures; and
3) sequence and structure evaluation using FiRES, HHrepID, lalign, RADAR, CE-symm, ReUPred and Swelfe with default parameter.

## Other benchmark databases 

The Dataset-non-TR (https://doi.org/10.1016/j.febslet.2015.08.025) contains duplicated domains.

![Structures with internal similarity in the database of no-tandem-repeats](images/No-tandem-repeats.png)

Some structures considered Asymmetric in the Internal symmetry dataset (https://doi.org/10.1371/journal.pcbi.1006842) have internal structure similarity.


![Structures with internal similarity in the domain_symm benchmark](images/Dom_symm_bench.jpg)

## References

1. Jha A, Flurchick KM, Bikdash M, Kc DB. Parallel-SymD : A Parallel Approach to Detect Internal Symmetry in Protein Domains. 2016;2016.
