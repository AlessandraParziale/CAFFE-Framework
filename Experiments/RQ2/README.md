# RQ2: Semantic Similarity Evaluation (Steps 2 and 3 of CAFFE)

This folder contains CSV files used in the evaluation of semantic similarity metrics and additional analyses conducted in the context of Research Question 2 (RQ2) of the CAFFE framework.

## Structure
```
Experiments/RQ2/
├── Visualizations/                        # Charts
│   └── ...                                
├── RQ2_Sampled_Prompts.csv                # Sampled test cases for RQ2 evaluation
├── RQ2_Responses.csv                      # LLM responses
├── RQ2_Responses_with_similarity.csv      # Responses + BERT, LSA, LDA similarity scores
├── global_fairness_bug_rates.csv          # Global fairness bug
├── Bias_specific_fairness_bug_rates.csv   # Fairness bug rates broken down by bias category
├── best_combinations_per_bias.csv         # Best metric–threshold
├── Summary_all_testcases.csv              # Aggregated PASS/FAIL
├── Summary_by_bias_type.csv               # PASS/FAIL counts split
├── Grouped_stats.csv                      # Summary stats
└── Overall_stats.csv                      # Statistical summary
```

## Contents

- **RQ2_Sampled_Prompts.csv** - Contains the sample of test cases selected for evaluation in RQ2.

- **RQ2_Responses.csv** - Contains the LLM responses to all the sampled test cases.

- **RQ2_Responses_with_similarity.csv** - Contains the LLM responses to all the test cases sampled alongside results for the three (BERT cosine similarity, LSA, and LDA) similarity metrics for each.

- **global_fairness_bug_rates.csv** - Contains the global number of fairness bugs detected, total test cases, and fail rates for each metric–threshold combination.
 
- **Bias_specific_fairness_bug_rates.csv** - Provides fairness bug counts and fail rates for each bias category, broken down by metric–threshold combination.

- **best_combinations_per_bias.csv** - Lists the best-performing metric and threshold for each bias type based on the number of FAILs.

- **Summary_all_testcases.csv** - Aggregated global performance results, including total PASS and FAIL counts, for all tested metric–threshold configurations.

- **Summary_by_bias_type.csv** - Detailed performance results split by bias type, including PASS and FAIL counts for each metric–threshold pair.

- **Grouped_stats.csv** - Summary statistics (mean, median, std, etc.) of semantic similarity scores grouped by bias type and metric.

- **Overall_stats.csv** - Statistical summary of similarity scores across all test cases, aggregated by metric.

## Visualizations
The folder **`Visualizations/`** provides additional charts containing the distributions and bias-specific barplots for the three similarity metrics.
