# Computational Practice: Accessing ENCODE Data Using Web Browser

## Lab Overview

The Encyclopedia of DNA Elements (ENCODE) project aims to build a comprehensive parts list of functional elements in the human genome, including elements that act at the protein and RNA levels, and regulatory elements that control cells and circumstances in which a gene is active. Since its launch in 2003, ENCODE has systematically mapped millions of candidate regulatory elements, many of which are biochemically active across hundreds of cell types and tissues. In this lab, you will learn to navigate the ENCODE portal to access, visualize, and download genomic data using only a web browser - no command line skills required!

The ENCODE portal provides an intuitive web interface to explore over 6,000 experiments across 600+ cell types and tissues. You'll discover how to find chromatin immunoprecipitation sequencing (ChIP-seq) data, DNase-seq experiments, RNA-seq datasets, and much more. Understanding how to access this treasure trove of functional genomics data is essential for modern genomics research.

## Lab Objectives:

In this lab, you will master the art of navigating the ENCODE data portal through your web browser. Specifically, you will:

* Navigate the ENCODE portal interface and understand its organization
* Search for specific datasets using filters and search terms
* Visualize genomic data using the ENCODE genome browser
* Download experimental data files and metadata
* Interpret quality metrics and experimental metadata
* Compare datasets across different cell types and experimental conditions

Follow these lab instructions:

## Task A: Navigate the ENCODE Portal and Understand Data Organization

### Step A1: Access the ENCODE Portal

1. Open your web browser and navigate to: https://www.encodeproject.org/
2. Familiarize yourself with the main navigation menu:
   - **Home**: Overview and recent updates
   - **Experiments**: Search interface for all ENCODE experiments
   - **Biosamples**: Information about cell types and tissues
   - **Datasets**: Processed data files and results
   - **Software**: Tools and pipelines used by ENCODE
   - **Help**: Documentation and tutorials

### Step A2: Explore the Data Matrix

1. Click on "Experiments" in the main navigation
2. This brings you to the ENCODE Data Matrix - a powerful search interface
3. Notice the left sidebar with filters including:
   - **Assay type**: ChIP-seq, DNase-seq, RNA-seq, etc.
   - **Biosample**: Cell types and tissues
   - **Target**: Specific proteins or histone marks
   - **Assembly**: Genome builds (GRCh38, hg19)
   - **Status**: Data processing status

### Step A3: Understanding ENCODE Data Types

Explore these key experimental categories by clicking on each in the "Assay type" filter:

1. **ChIP-seq**: Chromatin immunoprecipitation sequencing
   - Maps protein-DNA interactions
   - Identifies transcription factor binding sites
   - Maps histone modifications

2. **DNase-seq**: DNase I hypersensitivity sequencing
   - Identifies open chromatin regions
   - Reveals regulatory elements

3. **RNA-seq**: RNA sequencing
   - Measures gene expression
   - Identifies splice variants

4. **ATAC-seq**: Assay for transposase-accessible chromatin
   - Maps chromatin accessibility
   - Newer alternative to DNase-seq

## Task B: Search for Specific Datasets

### Step B1: Find ChIP-seq Data for a Transcription Factor

Let's search for CTCF (a key chromatin architecture protein) ChIP-seq data:

1. In the ENCODE Data Matrix, use these filters:
   - **Assay type**: Select "ChIP-seq"
   - **Target**: Type "CTCF" and select it
   - **Assembly**: Select "GRCh38" (latest human genome)
   - **Status**: Select "released"

2. Browse the results and note:
   - Number of experiments found
   - Variety of cell types tested
   - Different laboratories that contributed data

### Step B2: Focus on a Specific Cell Type

1. Add **Biosample** filter: Select "K562" (a leukemia cell line)
2. Click on one of the experiment entries
3. On the experiment page, examine:
   - **Experiment summary**: Basic information
   - **Documents**: Protocols and methods
   - **Files**: Raw and processed data
   - **Quality metrics**: Success indicators

### Step B3: Understanding File Types

In the "Files" section, you'll see different file types:
- **fastq.gz**: Raw sequencing reads
- **bam**: Aligned reads
- **bed**: Peak calls (genomic coordinates)
- **bigWig**: Coverage tracks for visualization
- **tsv**: Tabular data summaries

## Task C: Visualize Data in the Genome Browser

### Step C1: Launch the Genome Browser

1. From your CTCF ChIP-seq experiment page, find a **bigWig** file
2. Click the "Visualize" button next to the file
3. This launches the ENCODE genome browser with your data loaded

### Step C2: Navigate the Browser

1. **Search box**: Enter a gene name (try "MYC") or genomic coordinates
2. **Zoom controls**: Use +/- buttons or drag to zoom in/out
3. **Track controls**: Adjust signal height and visualization mode
4. **Add tracks**: Click "Add tracks" to load additional datasets

### Step C3: Compare Multiple Datasets

1. Search for the same region (MYC gene) in different cell types:
   - Add CTCF ChIP-seq from different cell lines
   - Add DNase-seq from the same cell types
   - Add RNA-seq expression data

2. Observe patterns:
   - Where does CTCF bind relative to the gene?
   - Are there cell-type specific differences?
   - How does chromatin accessibility correlate with CTCF binding?

## Task D: Download and Analyze Metadata

### Step D1: Download Experiment Metadata

1. Return to the ENCODE Data Matrix
2. Apply filters for your experiment of interest
3. Click "Download TSV" to get experiment metadata
4. Open the file in a spreadsheet program (Excel, Google Sheets)

### Step D2: Analyze the Metadata

Examine key columns:
- **Experiment accession**: Unique identifier (e.g., ENCSR000EUA)
- **Biosample**: Cell type or tissue
- **Target**: Protein or histone mark
- **Lab**: Research group that performed experiment
- **Date released**: When data became public
- **Audit results**: Quality control information

### Step D3: Quality Assessment

1. Look for experiments with:
   - **No audit errors**: High-quality data
   - **Good library complexity**: Sufficient unique reads
   - **Appropriate controls**: Necessary for ChIP-seq

2. Note any **audit warnings** or **errors** and understand their implications

## Task E: Explore Multi-omics Integration

### Step E1: Find Matched Datasets

1. Search for experiments from the same biosample (e.g., K562) with different assay types:
   - ChIP-seq for H3K4me3 (active promoter mark)
   - ChIP-seq for H3K27ac (active enhancer mark)
   - RNA-seq for gene expression
   - DNase-seq for chromatin accessibility

### Step E2: Integrated Analysis

1. Load these datasets in the genome browser
2. Navigate to a gene of interest (e.g., GAPDH, a housekeeping gene)
3. Compare the patterns:
   - H3K4me3 at the promoter?
   - H3K27ac at enhancers?
   - DNase hypersensitivity at regulatory elements?
   - RNA-seq expression level?

### Step E3: Hypothesis Generation

Based on your observations, formulate hypotheses:
- How do histone modifications correlate with gene expression?
- Are there regulatory elements outside the gene body?
- What distinguishes active from inactive genes?

## Task F: Advanced Features and Resources

### Step F1: Explore ENCODE Uniform Processing

1. Visit the **Pipelines** section
2. Understand how ENCODE standardizes data processing
3. Compare raw vs. processed data quality

### Step F2: Use ENCODE Search Tools

1. **ENCODE Search**: Advanced search across all metadata
2. **Experiment Matrix**: Visual representation of available data
3. **Biosample Matrix**: Compare cell types and tissues

### Step F3: Access Additional Resources

1. **ENCODE Data Standards**: Understanding file formats
2. **ENCODE Publications**: Key papers using ENCODE data
3. **ENCODE Tutorials**: Video guides for specific analyses

## Reflection Questions

After completing this lab, consider these questions:

1. **Data Scale**: How many experiments did you find for your target protein? What does this tell you about the comprehensiveness of ENCODE?

2. **Cell Type Specificity**: Did you observe differences in binding patterns between cell types? What might this mean biologically?

3. **Quality Control**: Why are quality metrics important in genomics experiments? What happens if you use low-quality data?

4. **Integration**: How can combining multiple data types (ChIP-seq, RNA-seq, DNase-seq) provide more insights than any single experiment?

5. **Future Directions**: What additional experiments would you design to test your hypotheses about gene regulation?

## Additional Resources

- **ENCODE Portal Help**: https://www.encodeproject.org/help/
- **ENCODE Data Standards**: https://www.encodeproject.org/data-standards/
- **ENCODE Publications**: https://www.encodeproject.org/publications/
- **Genome Browser Tutorial**: https://www.encodeproject.org/help/genome-browser/
- **ENCODE Data Interpretation Guide**: https://www.encodeproject.org/help/getting-started/
