# CAFFE-Framework

This is the online appendix of the paper _“Toward Systematic Counterfactual Fairness Evaluation of Large Language Models: The CAFFE Framework.”_ 

It provides a comprehensive framework for fairness testing of language models using counterfactual scenarios, along with experiments to evaluate its effectiveness.


## Structure
```
├── :file_folder: Caffe/        # Source code for the framework for fairness testing
    ├── :file_folder: KnowledgeBase
        ├── :page_facing_up: Crows_Pairs.csv
        ├── :page_facing_up: Knowledge_Base.csv
        ├── :page_facing_up: README.md
    ├── :page_facing_up: README.md
    ├── :page_facing_up: Step1-TestDataGenerator.ipynb
    ├── :page_facing_up: Step2(Example)-LLMResponsesGeneration.ipynb
    ├── :page_facing_up: Step3-ResponsesEvaluation.ipynb
├── :file_folder: Experiments/  # Experiments in Jupyter Notebooks
    ├── :file_folder: RQ1
        ├── :page_facing_up: README.md
        ├── :page_facing_up: RQ1_All_Generated_Prompts.csv
        ├── :page_facing_up: RQ1_Joined_Prompts_for_Evaluation.csv
        ├── :page_facing_up: RQ1_Optimal_Generated_Prompts.csv
        ├── :page_facing_up: RQ1_Results.csv
        ├── :page_facing_up: entropy_summary.csv
    ├── :file_folder: RQ2
        ├── :file_folder: GPT
            ├── :file_folder: Visualizations
                ├── :page_facing_up: BERT_Distribution.png
                ├── :page_facing_up: Barplots_Biases.png
                ├── :page_facing_up: LDA_Distribution.png
                ├── :page_facing_up: LSA_Distribution.png
            ├── :page_facing_up: RQ2_Responses_with_similarity.csv
            ├── :page_facing_up: RQ2_gpt_Answers.csv
            ├── :page_facing_up: best_combinations_per_bias.csv
            ├── :page_facing_up: bias_specific_fairness_bug_rates.csv
            ├── :page_facing_up: global_fairness_bug_rates.csv
            ├── :page_facing_up: grouped_stats.csv
            ├── :page_facing_up: overall_stats.csv
            ├── :page_facing_up: summary_all_testcases.csv
            ├── :page_facing_up: summary_by_bias_type.csv
        ├── :file_folder: LLAMA
            ├── :file_folder: Visualizations
                ├── :page_facing_up: BERT_Distribution.png
                ├── :page_facing_up: Barplots_Biases.png
                ├── :page_facing_up: LDA_Distribution.png
                ├── :page_facing_up: LSA_Distribution.png
            ├── :page_facing_up: RQ2_Responses_with_similarity.csv
            ├── :page_facing_up: RQ2_gpt_Answers.csv
            ├── :page_facing_up: best_combinations_per_bias.csv
            ├── :page_facing_up: bias_specific_fairness_bug_rates.csv
            ├── :page_facing_up: global_fairness_bug_rates.csv
            ├── :page_facing_up: grouped_stats.csv
            ├── :page_facing_up: overall_stats.csv
            ├── :page_facing_up: summary_all_testcases.csv
            ├── :page_facing_up: summary_by_bias_type.csv
        ├── :file_folder: MISTRAL
            ├── :file_folder: Visualizations
                ├── :page_facing_up: BERT_Distribution.png
                ├── :page_facing_up: Barplots_Biases.png
                ├── :page_facing_up: LDA_Distribution.png
                ├── :page_facing_up: LSA_Distribution.png
            ├── :page_facing_up: RQ2_Responses_with_similarity.csv
            ├── :page_facing_up: RQ2_gpt_Answers.csv
            ├── :page_facing_up: best_combinations_per_bias.csv
            ├── :page_facing_up: bias_specific_fairness_bug_rates.csv
            ├── :page_facing_up: global_fairness_bug_rates.csv
            ├── :page_facing_up: grouped_stats.csv
            ├── :page_facing_up: overall_stats.csv
            ├── :page_facing_up: summary_all_testcases.csv
            ├── :page_facing_up: summary_by_bias_type.csv
        ├── :page_facing_up: README.md
        ├── :page_facing_up: RQ2_Sampled_Prompts.csv
    ├── :file_folder: RQ3
        ├── :file_folder: Results
            ├── :file_folder: GPT4o
                ├── :file_folder: Results
                    ├── :page_facing_up: ASR_Result_GPT4o_Responses_RQ3_QandA_Test_Data_Joined.csv
                    ├── :page_facing_up: ASR_Result_GPT4o_Responses_RQ3_QandA_Test_Data_Joined.csv
                    ├── :page_facing_up: ASR_Result_GPT4o_Responses_RQ3_TD_Test_Data_Joined.csv.csv
                    ├── :page_facing_up: Result_GPT4o_Responses_RQ3_SA_Test_Data_Joined.csv
                    ├── :page_facing_up: Result_GPT4o_Responses_RQ3_TD_Test_Data_Joined.csv
                    ├── :page_facing_up: Stats_Result_GPT4o_Responses_RQ3_QandA_Test_Data_Joined.csv
                    ├── :page_facing_up: Stats_Result_GPT4o_Responses_RQ3_SA_Test_Data_Joined.csv
                    ├── :page_facing_up: Stats_Result_GPT4o_Responses_RQ3_TD_Test_Data_Joined.csv
                    ├── :page_facing_up: TSR_Result_GPT4o_Responses_RQ3_QandA_Test_Data_Joined.csv
                    ├── :page_facing_up: TSR_Result_GPT4o_Responses_RQ3_SA_Test_Data_Joined.csv
                    ├── :page_facing_up: TSR_Result_GPT4o_Responses_RQ3_TD_Test_Data_Joined.csv
                ├── :page_facing_up: GPT4o_Responses_RQ3_QandA_Test_Data_Joined.csv
                ├── :page_facing_up: GPT4o_Responses_RQ3_SA_Test_Data_Joined.csv
                ├── :page_facing_up: GPT4o_Responses_RQ3_TD_Test_Data_Joined.csv
            ├── :file_folder: LLaMa2
                ├── :file_folder: Results
                    ├── :page_facing_up: ASR_Result_LLAMA_Responses_RQ3_QandA_Test_Data_Joined.csv
                    ├── :page_facing_up: ASR_Result_LLAMA_Responses_RQ3_QandA_Test_Data_Joined.csv
                    ├── :page_facing_up: ASR_Result_LLAMA_Responses_RQ3_TD_Test_Data_Joined.csv.csv
                    ├── :page_facing_up: Result_LLAMA_Responses_RQ3_SA_Test_Data_Joined.csv
                    ├── :page_facing_up: Result_LLAMA_Responses_RQ3_TD_Test_Data_Joined.csv
                    ├── :page_facing_up: Stats_Result_LLAMA_Responses_RQ3_QandA_Test_Data_Joined.csv
                    ├── :page_facing_up: Stats_Result_LLAMA_Responses_RQ3_SA_Test_Data_Joined.csv
                    ├── :page_facing_up: Stats_Result_LLAMA_Responses_RQ3_TD_Test_Data_Joined.csv
                    ├── :page_facing_up: TSR_Result_LLAMA_Responses_RQ3_QandA_Test_Data_Joined.csv
                    ├── :page_facing_up: TSR_Result_LLAMA_Responses_RQ3_SA_Test_Data_Joined.csv
                    ├── :page_facing_up: TSR_Result_LLAMA_Responses_RQ3_TD_Test_Data_Joined.csv
                ├── :page_facing_up: LLAMA_Responses_RQ3_QandA_Test_Data_Joined.csv
                ├── :page_facing_up: LLAMA_Responses_RQ3_SA_Test_Data_Joined.csv
                ├── :page_facing_up: LLAMA_Responses_RQ3_TD_Test_Data_Joined.csv
            ├── :file_folder: MISTRAL
                ├── :file_folder: Results
                    ├── :page_facing_up: ASR_Result_MISTRAL_Responses_RQ3_QandA_Test_Data_Joined.csv
                    ├── :page_facing_up: ASR_Result_MISTRAL_Responses_RQ3_QandA_Test_Data_Joined.csv
                    ├── :page_facing_up: ASR_Result_MISTRAL_Responses_RQ3_TD_Test_Data_Joined.csv.csv
                    ├── :page_facing_up: Result_MISTRAL_Responses_RQ3_SA_Test_Data_Joined.csv
                    ├── :page_facing_up: Result_MISTRAL_Responses_RQ3_TD_Test_Data_Joined.csv
                    ├── :page_facing_up: Stats_Result_MISTRAL_Responses_RQ3_QandA_Test_Data_Joined.csv
                    ├── :page_facing_up: Stats_Result_MISTRAL_Responses_RQ3_SA_Test_Data_Joined.csv
                    ├── :page_facing_up: Stats_Result_MISTRAL_Responses_RQ3_TD_Test_Data_Joined.csv
                    ├── :page_facing_up: TSR_Result_MISTRAL_Responses_RQ3_QandA_Test_Data_Joined.csv
                    ├── :page_facing_up: TSR_Result_MISTRAL_Responses_RQ3_SA_Test_Data_Joined.csv
                    ├── :page_facing_up: TSR_Result_MISTRAL_Responses_RQ3_TD_Test_Data_Joined.csv
                ├── :page_facing_up: MISTRAL_Responses_RQ3_QandA_Test_Data_Joined.csv
                ├── :page_facing_up: MISTRAL_Responses_RQ3_SA_Test_Data_Joined.csv
                ├── :page_facing_up: MISTRAL_Responses_RQ3_TD_Test_Data_Joined.csv
            ├── :page_facing_up: RQ3_Results_GPT4o_Responses_RQ3_QandA_Test_Data_Joined.csv
            ├── :page_facing_up: RQ3_Results_GPT4o_Responses_RQ3_SA_Test_Data_Joined.csv
            ├── :page_facing_up: RQ3_Results_GPT4o_Responses_RQ3_TD_Test_Data_Joined.csv
            ├── :page_facing_up: RQ3_Results_LLAMA_Responses_RQ3_QandA_Test_Data_Joined.csv
            ├── :page_facing_up: RQ3_Results_LLAMA_Responses_RQ3_SA_Test_Data_Joined.csv
            ├── :page_facing_up: RQ3_Results_LLAMA_Responses_RQ3_TD_Test_Data_Joined.csv
            ├── :page_facing_up: RQ3_Results_MISTRAL_Responses_RQ3_QandA_Test_Data_Joined.csv
            ├── :page_facing_up: RQ3_Results_MISTRAL_Responses_RQ3_SA_Test_Data_Joined.csv
            ├── :page_facing_up: RQ3_Results_MISTRAL_Responses_RQ3_TD_Test_Data_Joined.csv
        ├── :page_facing_up: README.md
        ├── :page_facing_up: RQ3_All_Test_Data.csv
        ├── :page_facing_up: RQ3_All_Test_Data_Joined.csv
        ├── :page_facing_up: RQ3_QandA_Test_Data.csv
        ├── :page_facing_up: RQ3_SA_Test_Data.csv
        ├── :page_facing_up: RQ3_TD_Test_Data.csv
    ├── :page_facing_up: Experiments_ResearchQuestions.ipynb
    ├── :page_facing_up: README.md
├── :page_facing_up: README.md
```

The full implementation of the **CAFFE** framework is shared in the Caffe/ directory. The source code in Jupyter Notebook is commented to support the reusability and reproducibility of the framework.

## Note
Each folder and subfolder includes a dedicated README file with specific instructions on how to run and use the components within the package.
