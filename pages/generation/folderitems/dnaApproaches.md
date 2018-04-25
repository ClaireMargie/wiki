---
title: DNA Analysis Approaches
permalink: nodeContent/subnodeContent/dnaApproaches.html
layout: plain
reviewers:  Genomics Core, Amy Paguirigan, Jordan Smith
---
This page contains an outline of the platforms and approaches used to produce various types of large scale data sets from DNA that are available through the Fred Hutch Genomics Core. Please remember that this is a general resource, and example cost estimates and read depth, etc will vary study to study. To answer any questions specific to your study, please contact the staff at the [Genomics Core](https://sharedresources.fredhutch.org/core-facilities/genomics](https://sharedresources.fredhutch.org/core-facilities/genomics){:target="_blank"}<!--_--> to describe the basics of your study, such as the sample types, numbers, goal datasets, and proposed platforms of interest.  

## 1. DNA Sequencing for Variant Analysis

#### Capture-Based Sequencing - Example:  Whole Exome Sequencing

Exome sequencing is primarily used for large scale surveying of a large portion of the genome typically such as all the coding regions, or coding regions plus UTRs, etc.  Other types of capture based sequencing panels exist as well that target more specific regions in the genome such as commonly mutated regions in cancer, etc.   Regardless of the region of interest, the DNA libraries sequenced are generated by using capture probes specific to the particular regions covered in the panel to enrich for these regions in the final DNA sequences.  In most approaches, the capture uses pools of oligonucleotides (or probes) bound to strepavidin magnetic beads, whose sequence has been designed to hybridize to exon regions. After binding to genomic DNA, these probes are pulled down and washed, allowing exon regions to be selectively sequenced.

To perform exome or other capture based sequencing, a series of issues are important to consider that are unique to each study.  These issues can be discussed in more detail in consultation with the Fred Hutch Genomics Core staff.  

* **Region of coverage:**

    * Manufacturers often have multiple types of capture probe panels that cover different regions of the genome.  Choose one that covers the regions of most interest to the study - not all "exomes" are the same set of genomic regions!

        * Examples include Agilent selling SureSelect Human exome kits for All Exons alone, OR plus UTRs, or COSMIC regions, or other custom additions.  

        * Illumina’s TruSeq DNA Exome kit will cover slightly different regions than the Agilent kits as well.   Genomics Core currently doesn’t offer this workflow.

        * NimbleGen SeqCap EZ cover offers  custom capture baits, Exome, and other bait sets.

* **Number of reactions per kit:**

    * Because reagents are bought in kits, the unused reactions will increase your total cost even though they may not be used for your study.  

        * For example the Agilent Human All Exon V6 kit is sold in groups of 16 or 96, while the Illumina TruSeq DNA Exome kit is sold in groups of 24 or 96.  NimbleGen is sold in multiple configurations and pricing tiers accordingly.

* **Multiplexing the capture, library preparation and sequencing:**

    *  The particular reagent kit chosen may have the option to multiplex the capture, reducing per-sample costs.  

    * The generation of a library also can be multiplexed and the particular barcode sequences used to identify the reads from different samples will need to be chosen in accordance with how they will be sequenced.

    * Sequencing options on the HiSeq 2500 include Rapid Run mode (2 lanes only), or the High Output mode (8 lanes), and how the libraries are split over these lanes can impact the per-sample costs, time-to-sequencing, and the upstream capture and library preparation steps.  

* **Input amount:**

    * Typically exome sequencing will require on the order of 50ng to 1ug of input DNA.

    * Choosing a Low Input kit has implications downstream and for your data quality, but conversely it may not be feasible to get reliable data from all the samples in a cohort using a standard Input kit.  

* **Mean Read Depth/Coverage:**

    * A mean read depth of 100X over exome regions is a fairly standard goal depth, and using Illumina’s Sequencing Calculator tool linked below in Available Resources is useful in understanding how multiplexing and sequencing layout impact sequencing depth and cost.

* **Costs:**

    * While exomes are less expensive to generate than whole genomes, due to the moderate coverage of the genome of interest, sequencing costs are higher than for more targeted panels.  

    * An example data set previously generated on average 100x coverage in the Fred Hutch Genomics Core, with a low input kit, and all capture and library preparation steps were done by Genomics staff (full service), was approximately $750 per sample.  However, given the above variables, the exact cost for a given study will vary.   

#### Amplicon Based Sequencing - Targeted DNA sequencing

As an alternative approach to exome sequencing, targeted sequencing panels can offer high read depth of specific genomic regions; available panels often focus on known genes of interest for a disease, actionable target genes, or genomic regions known to have prognostic significance.  Due to DNA secondary structure and PCR amplification efficiency, not all targeted regions will have the same coverage and this variability is larger than what is seen in capture based sequencing approaches. To ensure that all target regions have high enough coverage to confidently identify variants, each manufacturer will likely provide a statistic such as " > 500× coverage for > 95% of amplicons at > 5,000× average sequencing depth."  This means that <5% of the amplicons in the panel may have <500x coverage in the final dataset even if the entire library is sequenced at 5,000x mean depth.  Following the manufacturer’s instructions for deciding on the goal sequencing depth for targeted DNA sequencing is particularly important for the data to be as complete as possible.  

Here is a [tech note from Illumina](https://support.illumina.com/content/dam/illumina-marketing/documents/products/technotes/technote_optimizing_coverage_for_targeted_resequencing.pdf){:target="_blank"}<!--_--> about how targeted DNA sequencing panels are designed and sequenced to maximize the data quality and coverage when used.  Understanding how these panels perform as compared to whole genome or whole exome sequencing is valuable in identifying whether the data are likely to be useful for the study goals.  

* **Region of coverage:**

    * There are a wide variety of different types of regions that can be targeted with panels, such as the [TruSight panels from Illumina](https://www.illumina.com/products/trusight-panels.html){:target="_blank"}<!--_-->.  Choosing the regions you are most interested in to focus on can allow for larger sample sizes due to cost reductions.  

* **Number of reactions per kit:**

    * Because reagents are bought in kits, the unused reactions will increase your total cost even though they may not be used for your study.  Often panels come in groups of 24, 36 or 96

* **Sequencing considerations:**

    * If the panel area is relatively small (~kb’s not ~Mbs+), depending on the desired average read depth, it is sometimes possible to sequence targeted libraries on the MiSeq.  

    * Sequencing options on the HiSeq 2500 include Rapid Run mode (2 lanes only), or the High Output mode (8 lanes) and if enough samples are being sequenced, it may be feasible and cost effective to put the entire cohort onto a number of lanes on a HiSeq.  

* **Input amount:**

    * Typically targeted DNA sequencing will require less input DNA, on the order of 50ng to 1ug of input.

    * Choosing a lower input requirement kit has implications downstream and for your data quality, but conversely it may not be feasible to get reliable data from all the samples in a cohort.

* **Mean Read Depth/Coverage:**

    * Read depth for targeted panels is very dependent on the manufacturer and the particular panel of interest.  The panels themselves should come with recommended target sequencing depths and provide statistics about how many regions should be above some minimal threshold of read depth.  Choosing a target depth will depend on the study goals as well.   

* **Costs:**

    * Targeted panels provide lower cost data, but at the expense of genomic ranges which depending on the study goals, can be no great loss and provide the opportunity to get data from a much higher sample number.

    * The costs for these vary greatly based on the size of the covered region in the panel because this increases the sequencing costs of the libraries.  An example cost seen in the Genomics Core for full service library preparation and sequencing of a TruSight Myeloid sequencing panel (~141kb, relatively small) for 96 samples was approximately $200/sample.  

#### SMRT sequencing (PacBio)

Both exome and targeted approaches rely on short length sequencing reads that are computational reconstructed into a longer sequence file. PacBio's Single Molecule Real-time (SMRT) is an alternative to the short-read approach. SMRT offers single reads of 1-20kb of sequence, for sequencing the entire length of a single gene or a large genomic region.

#### Whole Genome Guidance
More to come about approaches to obtain and evaluate the logistics involved in using whole genome sequencing data in a research study.  

### Available Resources

* Genohub has a useful guide to exome sequencing approaches. The comparison chart of exome library preparations is of particular note:

    * Link: [Genohub's Guide to Exome Sequencing](https://genohub.com/exome-sequencing-library-preparation/){:target="_blank"}<!--_-->

* Illumina has several exome sequencing options, which are outlined in the link below.

    * Link: [Illumina Whole Exome Sequencing](https://www.illumina.com/techniques/sequencing/dna-sequencing/targeted-resequencing/exome-sequencing.html){:target="_blank"}<!--_-->

* Agilent also has several exome sequencing options, including a more clinically focused option.

    * Link : [Agilent Exome Sequencing ](https://www.genomics.agilent.com/en/SureSelect-DNA-Target-Enrichment-Baits-NEW/SureSelect-Human-All-Exon-V6/?cid=AG-PT-124&tabId=AG-PR-1308)

* Roche NimbleGen has several exome and other bait sets.

    * Link : [Roche NimbleGen Exome Sequencing](http://sequencing.roche.com/en/products-solutions/by-category/target-enrichment/hybridization.html)

* Illumina has a variety of ready-made targeted DNA sequencing panels. Users can also design custom panels.

    * Link: [Illumina Targeted Sequencing Panels](https://www.illumina.com/techniques/sequencing/dna-sequencing/targeted-resequencing/targeted-panels.html){:target="_blank"}<!--_-->

* Illumina has a sequencing depth calculator tool to estimate what type of depth to expect in certain combinations of setups.  Note, the Genomics Core has access to MiSeqs and HiSeq2500 in Rapid Run (2 lanes at a time), or High Output (8 lanes at a time) Modes

    * Link: [Illumina Sequencing Calculator](https://support.illumina.com/downloads/sequencing_coverage_calculator.html){:target="_blank"}<!--_-->

* PacBio Single Molecule Real-time (SMRT) technology enables long-read (>20kb) sequencing.

    * Link: [PacBio SMRT](http://www.pacb.com/smrt-science/smrt-sequencing/){:target="_blank"}<!--_-->

## 2. DNA Microarrays

For quantitative studies of known targets, microarrays can be a very useful alternative to sequencing. The Genomics Core offers SNP and methylation arrays.

### SNP Genotyping Arrays

More to come

### Methylation Arrays

More to come

### Available Resources

* Illumina SNP Microarrays.

    *  Link: [Illumina Genotyping Microarrays](https://www.illumina.com/techniques/popular-applications/genotyping.html){:target="_blank"}<!--_-->

* Illumina Methylation Microarrays.

    * Link: [Illumina Methylation Microarrays](https://www.illumina.com/techniques/microarrays/methylation-arrays.html){:target="_blank"}<!--_-->

## 3. DNA Sequencing for other analysis types

Another use of DNA sequencing is as part of another analysis involving upstream processing of the DNA in order to then interpret the DNA Sequencing results as part of an experimental condition such as looking at epigenetics or DNA-protein interactions.  These types of projects are even more study-specific but can be performed with the Fred Hutch Genomics Core as well.  

### Chromatin-immunoprecipitation Sequencing (ChIP-seq)

ChIP-seq combines chromatin immunoprecipitation (ChIP) with massively parallel DNA sequencing to identify the binding sites of DNA-associated proteins.

Please email FH username **dharmaproject** if you are interested in this type of genomics work OR if you are an expert who'd like to contribute, and we will pursue getting more content for you.

### Reduced representation bisulfite sequencing (RRBS)

RRBS uses a combination of CpG island-specific restriction enzymes with bisulfite sequencing to enrich for methylation sites before sequencing.

Please email FH username **dharmaproject** if you are interested in this type of genomics work OR if you are an expert who'd like to contribute, and we will pursue getting more content for you.

### Available Resources

* Epigenie has a useful guide to getting started with ChIP-seq.

    * Link: [Epigenie's Guide to ChIP-seq](http://epigenie.com/guide-getting-started-with-chip-seq/){:target="_blank"}<!--_-->

* The genomics core uses the Kapa Hyper Prep kit for ChiP-seq.

    * Link: [Kapa Hyper Prep for ChIP-seq](http://sequencing.roche.com/en/products-solutions/by-application/research/chip-sequencing.html){:target="_blank"}<!--_-->

* The Babraham Institute has a brief guide to the biology and bioinformatics of RRBS.

    * Link: [Babraham Institute's Brief Guide to RRBS](http://www.bioinformatics.babraham.ac.uk/projects/bismark/RRBS_Guide.pdf){:target="_blank"}<!--_-->

---

Latest Edit: Mar 29, 2018