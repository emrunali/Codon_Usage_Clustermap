# Codon_Usage_Clustermap
**Overview**
This project analyzes codon usage patterns across different genes and species, clustering them based on their codon usage frequencies. By leveraging publicly available nucleotide sequences, the study provides insights into codon preferences and their potential evolutionary relationships. The visualization of codon usage similarities helps to identify patterns across species and their genetic code adaptation.

**Purpose**
The primary goal of this project is to:
1. Compare codon usage across different species by analyzing their coding sequences (CDS).
2. Identify optimal codons for each amino acid, which could provide insights into translational efficiency.
3. Cluster species based on their codon usage to examine evolutionary and functional relationships.
4. Visualize codon usage trends using heatmaps and hierarchical clustering.
5. Provide a foundation for further research in gene expression, protein synthesis efficiency, and evolutionary biology.

**Tools & Libraries Used**
- Python
- BioPython (Bio.Entrez, Bio.SeqIO, Bio.Seq.CodonTable) – For fetching sequence data from NCBI and extracting CDS.
- Pandas – For data manipulation and analysis.
- Seaborn – For heatmap and clustering visualizations.
- Matplotlib – For graphical representation.

**Implementation**
1. Fetch genetic sequences: The script retrieves coding sequences (CDS) from GenBank using user-provided accession numbers.
2. Extract codons: The CDS is parsed, and codon frequencies are computed using a selected genetic code table.
3. Compute codon usage bias: The relative frequency of each codon per amino acid is calculated.
4. Identify optimal codons: The most frequently used codons per amino acid are determined.
5. Generate heatmaps and clustermaps: Codon usage patterns are visualized across multiple species.

**Example Usage**
1. Run the script and enter GenBank accession numbers when prompted.
2. Choose a genetic code table ID (1-33) for the species of choice.
3. The script will fetch sequences, compute codon usage, and generate visualizations.
```python codon_usage_analysis.py```

**Future Improvements**
1. Include Species Names: Instead of displaying only accession IDs, integrating species names will make the results more interpretable.
2. Incorporate scRNA-seq Data & Gene Expression Analysis:
   - Relate codon usage bias to gene expression levels.
   - Investigate how codon preference affects mRNA translation efficiency.
   - Compare tissue-specific expression levels and codon bias.
3. Codon Adaptation Index (CAI): Compute CAI to assess how closely a gene follows the optimal codon usage of a species.
4. Comparative Evolutionary Analysis: Use phylogenetic trees to study the relationship between species based on codon usage similarity.
5. Machine Learning for Codon Optimization: Train models to predict codon optimization for synthetic biology applications.

**Conclusion**
This project provides a foundation for codon usage analysis and its implications in evolutionary biology, translational efficiency, and gene expression regulation. Future expansions will allow deeper insights into how codon bias impacts protein synthesis across species and conditions.






References:
1. https://github.com/rhondene/Codon-Usage-in-Python/blob/master/aa_usage.py
2. https://www.biotite-python.org/examples/gallery/sequence/codon_usage.html
