Groupmember usernames: marilugar, leagschw2

Ribo-Seq (Ribosome Profiling) is an assay that measures which mRNAs are actively being translated into proteins by capturing ribosome-bound mRNA fragments. 
The technique "freezes" ribosomes in place on mRNAs, digests unprotected RNA, and sequences the small ribosome-protected fragments (RPFs), providing a high-resolution snapshot of translation activity.

Ribo-Seq is used to:
- Identify actively translated genes.
- Analyze translation efficiency and dynamics (e.g., ribosome positioning, pausing).
- Discover novel protein-coding regions and non-canonical open reading frames (ORFs).
- Study translational regulation under various conditions, such as during development, disease states (e.g., cancer), or stress responses.
- It is a valuable tool for understanding gene expression at the translational level, offering insights that go beyond traditional RNA-seq.

Sources:
1. https://www.science.org/doi/abs/10.1126/science.1168978
2. https://emea.illumina.com/techniques/sequencing/rna-sequencing/ribosome-profiling.html

Application: In cancer research, Ribo-Seq is widely used to understand how translation is deregulated in tumors. 

Statistical Methods Used:
1. Differential Translation Efficiency (TE) Analysis: identifies mRNAs whose translation efficiency (TE) changes between conditions (e.g., normal vs. cancerous tissue).
- Here, ratio of RPFs (ribosome-protected reads) are compared to RNA-seq reads for each gene. Statistical models such as generalized linear models (GLMs) are used to assess differential TE.
2. Peak Calling and Ribosome Density Profiling: identifies regions of mRNA where ribosomes are enriched, including novel translation start sites or ribosome pausing sites.
- Here, peak calling algorithms are used to detect areas of the transcript where ribosomes accumulate. Gaussian mixture models or kernel density estimation are often used to smooth and quantify ribosome density across transcripts.

3. Identification of Novel ORFs: identifies previously unannotated ORFs that are being actively translated.
- Here, Statistical tools, such as Harringtonine analysis (a method to study translation initiation) or ribosome initiation scanning models, can be applied to identify novel ORFs based on ribosome occupancy at unexpected regions.

4. Translational Pausing and Ribosome Stalling: identifies regions where ribosomes slow down or stall during translation.
- Here, cumulative statistical distributions and hidden Markov models (HMMs) are used to detect patterns of ribosome stalling, where certain codons or structural elements (e.g., secondary RNA structures) cause ribosomes to pause.
