# RQ1: Evaluation  of Research Question 1 (Step 1 of CAFFE)

This folder contains all outputs and intermediate files generated to evaluate the first step of the CAFFE framework.

## Contents
- **RQ1_All_Generated_Prompts.csv** - Contains the 20 prompt pairs created for each <triple, intent> combination.

- **RQ1_Joined_Prompts_for_Evaluation.csv** - Contains the 20 single prompts (not paired) for each <triple, intent>. This format is used to compute Shannon entropy with Miller–Madow correction on individual prompts.

- **entropy_summary.csv**  - Summarizes the Shannon entropy with Miller–Madow calculated for each set of 20 prompts.

- **RQ1_Results.csv** - Aggregates the entropy analysis results: provides mean, median, and standard deviation of Shannon entropy with Miller–Madow. The median entropy of 12 was selected as the optimal number of prompts.

- **RQ1_Optimal_Generated_Prompts.csv** . Contains the final selection of generated prompts, 12 prompt pairs per <triple, intent>.
