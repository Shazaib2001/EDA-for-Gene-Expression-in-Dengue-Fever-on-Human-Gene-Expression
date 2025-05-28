# EDA-for-Gene-Expression-in-Dengue-Fever-on-Human-Gene-Expression

#Project overview

This project presents a comprehensive exploratory analysis of gene expression across the clinical spectrum of Dengue infection using the GEO dataset GDS5093. The dataset includes samples from patients with Dengue Fever (DF), Dengue Haemorrhagic Fever (DHF), individuals in the recovery (convalescent) phase, and healthy controls. Through dimensionality reduction, clustering, differential expression analysis, and machine learning, this study aims to uncover distinct transcriptional signatures associated with disease severity, progression, and recovery. The analysis identifies potential biomarkers and evaluates a classification model to distinguish between DF and DHF, offering insights into the molecular pathology of Dengue and directions for diagnostic and therapeutic research.

#Data Source and Description

This project utilises the gene expression dataset GDS5093 from the NCBI Gene Expression Omnibus (GEO). The dataset contains microarray data derived from whole blood samples of 28 individuals affected by different stages of Dengue infection, collected in Bangkok.

The dataset includes four distinct clinical groups:

Dengue Fever (DF): Patients with classical dengue symptoms.

Dengue Haemorrhagic Fever (DHF): Patients exhibiting severe complications such as vascular permeability and bleeding.

Convalescent (COV): Individuals recovering from dengue infection, offering insight into post-infection recovery processes.

Healthy Controls (HC): Uninfected individuals serving as a baseline for gene expression comparison.
This dataset enables systematic analysis of transcriptional responses to Dengue virus infection and allows for the identification of biomarkers across the disease spectrum.

#Analysis Techniques Used

Principal Component Analysis (PCA): Used to reduce dimensionality and identify the main sources of variance in the data, facilitating the separation of disease states based on transcriptional signatures.

Hierarchical Cluster Analysis (HCA): Applied to detect natural groupings among samples and genes. Dendrograms were used to visually interpret similarities in gene expression profiles across the clinical groups.

Differential Expression Analysis: Conducted using t-tests and fold-change calculations to compare gene expression between groups (e.g., convalescent vs. healthy, DF vs. DHF). Volcano plots were generated to visualise significantly regulated genes.

Support Vector Machine (SVM) Classification: A supervised learning algorithm trained to differentiate between DF and DHF cases. Model performance was evaluated using classification reports, confusion matrices, bootstrap accuracy estimation, and permutation testing to assess statistical significance.

#Results

PCA showed that PC1 and PC2 captured ~30% of the total variance, effectively separating DHF samples from other groups.

HCA identified clear clustering patterns, with DHF samples forming a distinct, homogeneous group.

Volcano plots revealed significant gene expression differences between the Convalescent and Healthy groups, with genes like CAMK1D and BAG1 notably altered.

SVM classifier achieved ~62.67% accuracy in distinguishing DF from DHF. However, permutation testing (p = 0.578) indicated the result was not statistically significant.

#Installation

pip install pandas numpy matplotlib seaborn scikit-learn scipy bootstrapped

#Usage

Run the analysis scripts provided in the repository to replicate the study or apply the methods to new gene expression datasets. Ensure your input data follows a similar format to GEO dataset GDS5093, and adjust file paths as needed.

#Contributing

Contributions are welcome. Please fork the repository and submit pull requests with your suggested improvements or additional features.

#License

This project is licensed under the MIT License.

#Contact

For queries, please contact Shazaib Rehman.
Connect with me on LinkedIn.



