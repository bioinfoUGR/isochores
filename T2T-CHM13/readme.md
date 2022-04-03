## Isochores in T2T gap-free human genome from the CHM13 cell line

CHM13hTERT cells were grown in culture from one such conception at Magee-Women’s Hospital (Pittsburgh, PA). Cryogenically frozen cells from this culture were grown and transformed using human telomerase reverse transcriptase (hTERT) to develop a cell line. This cell line retains a 46,XX karyotype and near-complete homozygosity [1]

On this directory, you can find the coordinates of the isochores predicted by IsoFinder [2] in the complete gap-free human genome obtained by the Telomere-to-Telomere (T2T) consortium in the cell line T2T-CHM13 [1]. Chromosome FASTA sequences were obtained from the GenBank assembly accession GCA_009914755.4 (GCA_009914755.4_T2T-CHM13v2.0_genomic.fna.gz).

### IsoFinder sintax

`isofinder <DNA FASTA file> <Sig.Level> <Sig.Method> <Coarse-graining level> <File out>`

#### Used values for the parameters
  
1. Significance level: 0.95 
2. Significance method: p3 (Parametric for maximum value)
3. Coarse-graining level: 3000

#### Output (chr_T2T-CHM13_iso.zip: https://github.com/bioinfoUGR/isochores/blob/main/T2T-CHM13/chr_T2T-CHM13_iso.zip)

Isochore coordinates for each chromosome are output to a BED formatted text file with the following fields:
1.	chrom - The name of the chromosome (e.g. chr3, chrX…).
2.	chromStart - The starting position of the isochore in the chromosome.
3.	chromEnd - The ending position of the isochore in the chromosome. 
4.	name - The name of the isochore.
5.	score - A score between 0 and 1000, indicating the level of gray in which this isochore may be displayed (higher numbers = darker gray) in a graphical representation (e.g. UCSC Genome Browser)
6.	strand - Defines the strand. Either "." (=no strand) or "+" or "-".

<img src="https://user-images.githubusercontent.com/8526974/161422809-0045fb9c-0484-48e7-814c-8f327bf0904e.png" width="500">

### References

[1] Sergey Aganezov et al. (2022) A complete reference genome improves analysis of human genetic variation, Science, 376, 6588. https://doi.org/10.1126/science.abl3533

[2] Oliver JL, Carpena P, Hackenberg M, Bernaola-Galván P. 2004. IsoFinder: computational prediction of isochores in genome sequences. Nucleic Acids Research 32: W287-W292. http://dx.doi.org/10.1093/nar/gkh399



