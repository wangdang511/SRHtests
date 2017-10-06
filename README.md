# SRH analysis pipeline

1. run ```start_over.sh``` to clean out any old results

2. run ```srh.py``` to get SRH stats and IQtree input files for all datasets in raw_data

3. run ```run_iqtree.sh``` to run IQ tree on all the folders from 2 (everything in ```processed_data/IQtree```)

4. run ```tree_dist.r``` this creates ```processed_data/tree_distances.csv``` which is a CSV file of tree-to-tree path distances comparing all three trees generated from each of the tree tests for each dataset. 

5. run `charsets_percentage.py` to generate a table that contains the percentage of the Bad and Not-Bad character sets in each data set

7. run `charset_length.py`to generate a table that contains the length of each character set in each data set 

8. run `is_charset_bad.py` to generate a table that divides the character sets into two categories: one that rejects the null hypothesis and one that does not

9. run `trees_lengths.py` to generate a table that contains the lengths of the trees generated by IQtree from each partition (all, bad, not_bad) and symmetry test (MPTS, MPTMS, MPTIS)

10. run `topology_tests.py` to generate a table that contains all the topology tests results

11. run `figure1.r`

12. run `figure2.r`

13. run `figure3.r`