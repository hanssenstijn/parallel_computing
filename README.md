# Assignment 3 parallel_computing

`Script.rmd` represents the R notebook. The notebook describes: using parralel computing when importing molecular descriptors.

The structured data file that has been used contains molecules information related to BRCA1 Expression. It can be downloaded from PubChem Assay: [AID624202](https://pubchem.ncbi.nlm.nih.gov/bioassay/624202), Download > Tested Substances > Structures SDF.

For the reason of computational time and power, only a subset of molecules is selected too in parallel compute their discriptors. This calculation was done using half of the available cores (n = 2) and maximum minus 1 (n = 3).

The script will convert the molecules into smiles and then by each different core will the smiles be parse back into molecules. This has to be done in order to make the parallel computing to happen.