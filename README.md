# Internal_structure_similarity_benchmark

We constructed a database of proteins without internal sequence and structure similarity. 
To this end, we used three sequential filters:

a database of non-symmetrical protein structures was constructed. To this
end, a subset of the PDB composed of 28337 non-redundant chains, as determined by BLASTClust
at 30% sequence identity, 
was evaluated by SymD31. From a total of 6088 structures that were
considered non-symmetrical (Z-score < 4), 3300 were randomly selected to continue to the next
stage. Then, two random groups were assembled with 300 and 3000 proteins to resemble the sizes
of MALIDUP and RepeatsDB, respectively. The second filter consisted in excluding proteins that
presented repeated sequence signatures according to InterPro46. These signatures include
annotations from CATH47, Gene3D48, CDD49, PANTHER50, Pfam51, ProDom52, PROSITE53
,
SMART54, SUPERFAMILY55 and TIGRFAMs56. The remaining proteins were evaluated by all
algorithms tested in this work (see performance evaluation). Pairwise structure alignments of the
predictions made by any of the tested algorithms were performed with TM-align. Predicted repeat
pairs with more than 15 aligned residues and a TM-score higher than 0.5 were visually inspected to
evaluate the content, connectivity and orientation of their SSEs. This inspection revealed the
presence of 81 proteins with internal structure similarity, which were removed from the final
control sets (Suppl. Table 1). Finally, two control sets, integrated by 132 and 2125 proteins with
low probability of containing repeated elements, were established as negative controls for
MALIDUP and RepeatsDB, respectively.

# Other benchmark databases 

The Dataset-non-TR (https://doi.org/10.1016/j.febslet.2015.08.025) contains duplicated domains.

![Structures with internal similarity in the database of no-tandem-repeats](images/No-tandem-repeats.png)

Some structures considered Asymmetric in the Internal symmetry dataset (https://doi.org/10.1371/journal.pcbi.1006842) have internal structure similarity.


![Structures with internal similarity in the domain_symm benchmark](images/Dom_symm_bench.jpg)
