## Isochores in T2T gap-free human genome from the CHM13 cell line

CHM13hTERT cells were grown in culture from one such conception at Magee-Women’s Hospital (Pittsburgh, PA). Cryogenically frozen cells from this culture were grown and transformed using human telomerase reverse transcriptase (hTERT) to develop a cell line. This cell line retains a 46,XX karyotype and near-complete homozygosity [1]

The genome of CHM13hTERT human cell line was sequenced with a number of technologies (https://github.com/marbl/CHM13). Human genomic DNA was extracted from the cultured cell line. As the DNA is native, modified bases will be preserved. The data includes 30x PacBio HiFi, 120x coverage of Oxford Nanopore, 70x PacBio CLR, 50x 10X Genomics, as well as BioNano DLS and Arima Genomics HiC.

On this directory, you can find the coordinates of the isochores predicted by IsoFinder [2] (https://github.com/bioinfoUGR/isofinder) in the complete gap-free human genome obtained by the Telomere-to-Telomere (T2T) consortium in the cell line T2T-CHM13 [1]. Chromosome FASTA sequences were obtained from the GenBank assembly accession GCA_009914755.4 (GCA_009914755.4_T2T-CHM13v2.0_genomic.fna.gz).

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

Isochore legths
|chrom|N|Min|Median|Max|
|-----|-|---|------|---|
|chr1|1113|30004| 102,983   | 5,403,580|
|chr2|897|30004| 128,804   | 4,304,270|   
|chr3|656|30004| 127,485   | 5,001,190|   
|chr4|427|30004| 234,223   | 5,642,550|   
|chr5|561|30004| 164,800   | 7,206,270|   
|chr6|510|30004| 163,262   | 3,500,380|   
|chr7|596|30004| 119,830   | 3,412,220|   
|chr8|449|30004| 147,916   | 4,875,420|   
|chr9|501|30004| 107,885   | 22,256,800|   
|chr10|562|30004| 121,504   | 3,195,210|   
|chr11|551|30004| 109,143   | 3,008,680|   
|chr12|505|30005| 115,060   | 3,649,550|   
|chr13|317|30004| 128,955   | 10,449,500|   
|chr14|426|30004| 101,284   | 3,881,480|   
|chr15|461|30004| 104,795   | 7,482,370|   
|chr16|457|30004| 82,508   | 12,645,100|  
|chr17|517|30004| 82,785   | 4,713,850|   
|chr18|237|30004| 180,918   | 3,584,850|   
|chr19|313|30004| 101,006   | 2,676,290|   
|chr20|314|30004| 101,682   | 2,232,290|   
|chr21|178|30004| 95,755   | 4,852,870|   
|chr22|342|30004| 68,700   | 1,690,830|   
|chrX|366|30004| 166,946   | 14,835,700|   


<img src="https://user-images.githubusercontent.com/8526974/161422809-0045fb9c-0484-48e7-814c-8f327bf0904e.png" width="500">

### References

[1] Sergey Aganezov et al. (2022) A complete reference genome improves analysis of human genetic variation, Science, 376, 6588. https://doi.org/10.1126/science.abl3533

[2] Oliver JL, Carpena P, Hackenberg M, Bernaola-Galván P. 2004. IsoFinder: computational prediction of isochores in genome sequences. Nucleic Acids Research 32: W287-W292. http://dx.doi.org/10.1093/nar/gkh399



