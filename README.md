# Biopython + pandas Mini Pipeline

Today I combined **Biopython + pandas** to build a small real-world bioinformatics workflow.

## 📌 Task
Analyze FASTA sequences and create a filtered gene table.

## ⚙️ Steps Performed
1. Read FASTA using Biopython (SeqIO)
2. Compute:
   - sequence length
   - GC %
3. Store results in pandas DataFrame
4. Filter genes (length and GC thresholds)
5. Export results to CSV

## 📂 Files Added

A_pipeline/a1_pipeline.py  
→ End-to-end FASTA → statistics → filtered CSV pipeline  

A_pipeline/genes.fasta  
→ Input sequences  

A_pipeline/gene_filtered.csv  
→ Filtered output table  

## ▶️ Run

```bash
cd panda/A_pipeline
python a1_pipeline.py
```

## ✅ Skills Practiced
- Sequence parsing (Biopython)
- DataFrames (pandas)
- Data filtering
- CSV export
- Building mini bioinformatics pipelines

---

# 📊 Data Visualization (matplotlib)

After generating the filtered gene table, I visualized the data using **matplotlib**.

## Script
A_pipeline/a2_plot.py

## What it does
Reads `gene_filtered.csv` and creates plots:

1. Gene Length Distribution → `length_hist.png`
2. GC% Distribution → `gc_hist.png`
3. Length vs GC Scatter Plot → `length_vs_gc.png`

## ▶️ Run

```bash
cd panda/A_pipeline
python a2_plot.py
```

## 📈 Output Files

- length_hist.png
- gc_hist.png
- length_vs_gc.png

## Skills Practiced

- Reading CSV with pandas
- Histogram plotting
- Scatter plots
- Saving figures automatically
- Basic biological data visualization
