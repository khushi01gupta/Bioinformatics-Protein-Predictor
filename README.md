APOE SNP Analyzer: Genetic Risk Simulation
Project Overview

This Python-based bioinformatics tool simulates personalized genetic risk assessment by analyzing Single Nucleotide Polymorphisms (SNPs). Specifically, it targets the rs429358 locus on the APOE gene, which is a primary genetic determinant of late-onset Alzheimer’s disease.

This project demonstrates how conditional logic is applied to genomic data to translate raw genotypes into clear clinical risk interpretations.

Biological Context: The APOE Gene

The APOE gene provides instructions for producing apolipoprotein E, a protein that combines with fats in the body to form lipoproteins. The variant at the rs429358 locus determines the presence of the ε4 allele.

Genotype Risk Mapping

Genotype	Alleles	Risk Phenotype	Clinical Interpretation
E4/E4	CC	Significantly Increased	Highest genetic risk; two copies of the risk allele.
E3/E4	TC	Increased	Elevated risk; one copy of the ε4 allele present.
E3/E3	TT	Typical	Baseline population risk; the most common genotype.
Features

Genotype Parsing: Validates and processes user-provided SNP data.

Risk Logic Engine: Maps specific allele combinations to established clinical risk categories.

Bioinformatics Reporting: Generates a structured clinical report within the terminal.

Getting Started

Prerequisites

Python 3.x (This is a lightweight version and does not require external libraries like pandas or Biopython).

Installation

Clone this repository: git clone https://github.com/yourusername/apoe-snp-analyzer.git

Navigate to the directory: cd apoe-snp-analyzer

Running the Analyzer Open the script and modify the patient_input variable to test different genotypes. For example: patient_input = 'TC'

Then run the program: python apoe_analyzer.py

Sample Output

Plaintext
==================================================
        APOE SNP ANALYZER: CLINICAL REPORT
==================================================
Locus:             rs429358 (APOE)
Genotype detected: TC
Allele 1:          T (Threonine)
Allele 2:          C (Cysteine)
--------------------------------------------------
RESULT:            E3/E4
RISK LEVEL:        INCREASED RISK
--------------------------------------------------
NOTES:
The presence of a single C (Cysteine) allele at this 
locus indicates the E4 variant, which is associated 
with an increased risk of Alzheimer's compared to 
the baseline E3/E3 population.
==================================================
Medical Disclaimer

This tool is intended for educational and simulation purposes only. Genetic risk is multifactorial; the presence of an ε4 allele does not guarantee an Alzheimer's diagnosis, nor does its absence guarantee immunity. This software should not be used for medical diagnosis or clinical decision-making.
