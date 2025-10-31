# CAFFE-Framework

This is the online appendix of the paper _“Toward Systematic Counterfactual Fairness Evaluation of Large Language Models: The CAFFE Framework.”_ 

It provides a comprehensive framework for fairness testing of language models using counterfactual scenarios, along with experiments to evaluate its effectiveness.


## Structure
The repository is organized as follows:

```
├── 📁 Caffe                      # Source code for the framework for fairness testing
    ├── 📁 KnowledgeBase
        ├── 📄 Crows_Pairs.csv
        ├── 📄 Knowledge_Base.csv
        ├── 📄 README.md
    ├── 📄 README.md
    ├── 📄 Step1-TestDataGenerator.ipynb
    ├── 📄 Step2(Example)-LLMResponsesGeneration.ipynb
    ├── 📄 Step3-ResponsesEvaluation.ipynb
├── 📁 Experiments                    # Experiments in Jupyter Notebooks
    ├── 📁 RQ1
        ├── 📄 README.md
        ├── 📄 RQ1_All_Generated_Prompts.csv
        ├── 📄 RQ1_Joined_Prompts_for_Evaluation.csv
        ├── 📄 RQ1_Optimal_Generated_Prompts.csv
        ├── 📄 RQ1_Results.csv
        ├── 📄 entropy_summary.csv
    ├── 📁 RQ2
        ├── 📁 GPT
            ├── 📁 Visualizations
                ├── 📄 BERT_Distribution.png
                ├── 📄 Barplots_Biases.png
                ├── 📄 LDA_Distribution.png
                ├── 📄 LSA_Distribution.png
            ├── 📄 RQ2_Responses_with_similarity.csv
            ├── 📄 RQ2_gpt_Answers.csv
            ├── 📄 best_combinations_per_bias.csv
            ├── 📄 bias_specific_fairness_bug_rates.csv
            ├── 📄 global_fairness_bug_rates.csv
            ├── 📄 grouped_stats.csv
            ├── 📄 overall_stats.csv
            ├── 📄 summary_all_testcases.csv
            ├── 📄 summary_by_bias_type.csv
        ├── 📁 LLAMA
            ├── 📁 Visualizations
                ├── 📄 BERT_Distribution.png
                ├── 📄 Barplots_Biases.png
                ├── 📄 LDA_Distribution.png
                ├── 📄 LSA_Distribution.png
            ├── 📄 RQ2_Responses_with_similarity.csv
            ├── 📄 RQ2_gpt_Answers.csv
            ├── 📄 best_combinations_per_bias.csv
            ├── 📄 bias_specific_fairness_bug_rates.csv
            ├── 📄 global_fairness_bug_rates.csv
            ├── 📄 grouped_stats.csv
            ├── 📄 overall_stats.csv
            ├── 📄 summary_all_testcases.csv
            ├── 📄 summary_by_bias_type.csv
        ├── 📁 MISTRAL
            ├──  📁 Visualizations
                ├── 📄 BERT_Distribution.png
                ├── 📄 Barplots_Biases.png
                ├── 📄 LDA_Distribution.png
                ├── 📄 LSA_Distribution.png
            ├── 📄 RQ2_Responses_with_similarity.csv
            ├── 📄 RQ2_gpt_Answers.csv
            ├── 📄 best_combinations_per_bias.csv
            ├── 📄 bias_specific_fairness_bug_rates.csv
            ├── 📄 global_fairness_bug_rates.csv
            ├── 📄 grouped_stats.csv
            ├── 📄 overall_stats.csv
            ├── 📄 summary_all_testcases.csv
            ├── 📄 summary_by_bias_type.csv
        ├── 📄 README.md
        ├── 📄 RQ2_Sampled_Prompts.csv
    ├── 📁 RQ3
        ├── 📁 Results
            ├── 📁 GPT4o
                ├── 📁 Results
                    ├── 📄 ASR_Result_GPT4o_Responses_RQ3_QandA_Test_Data_Joined.csv
                    ├── 📄 ASR_Result_GPT4o_Responses_RQ3_QandA_Test_Data_Joined.csv
                    ├── 📄 ASR_Result_GPT4o_Responses_RQ3_TD_Test_Data_Joined.csv.csv
                    ├── 📄 Result_GPT4o_Responses_RQ3_SA_Test_Data_Joined.csv
                    ├── 📄 Result_GPT4o_Responses_RQ3_TD_Test_Data_Joined.csv
                    ├── 📄 Stats_Result_GPT4o_Responses_RQ3_QandA_Test_Data_Joined.csv
                    ├── 📄 Stats_Result_GPT4o_Responses_RQ3_SA_Test_Data_Joined.csv
                    ├── 📄 Stats_Result_GPT4o_Responses_RQ3_TD_Test_Data_Joined.csv
                    ├── 📄 TSR_Result_GPT4o_Responses_RQ3_QandA_Test_Data_Joined.csv
                    ├── 📄 TSR_Result_GPT4o_Responses_RQ3_SA_Test_Data_Joined.csv
                    ├── 📄 TSR_Result_GPT4o_Responses_RQ3_TD_Test_Data_Joined.csv
                ├── 📄 GPT4o_Responses_RQ3_QandA_Test_Data_Joined.csv
                ├── 📄 GPT4o_Responses_RQ3_SA_Test_Data_Joined.csv
                ├── 📄 GPT4o_Responses_RQ3_TD_Test_Data_Joined.csv
            ├── 📁 LLaMa2
                ├── 📁 Results
                    ├── 📄 ASR_Result_LLAMA_Responses_RQ3_QandA_Test_Data_Joined.csv
                    ├── 📄 ASR_Result_LLAMA_Responses_RQ3_QandA_Test_Data_Joined.csv
                    ├── 📄 ASR_Result_LLAMA_Responses_RQ3_TD_Test_Data_Joined.csv.csv
                    ├── 📄 Result_LLAMA_Responses_RQ3_SA_Test_Data_Joined.csv
                    ├── 📄 Result_LLAMA_Responses_RQ3_TD_Test_Data_Joined.csv
                    ├── 📄 Stats_Result_LLAMA_Responses_RQ3_QandA_Test_Data_Joined.csv
                    ├── 📄 Stats_Result_LLAMA_Responses_RQ3_SA_Test_Data_Joined.csv
                    ├── 📄 Stats_Result_LLAMA_Responses_RQ3_TD_Test_Data_Joined.csv
                    ├── 📄 TSR_Result_LLAMA_Responses_RQ3_QandA_Test_Data_Joined.csv
                    ├── 📄 TSR_Result_LLAMA_Responses_RQ3_SA_Test_Data_Joined.csv
                    ├── 📄 TSR_Result_LLAMA_Responses_RQ3_TD_Test_Data_Joined.csv
                ├── 📄 LLAMA_Responses_RQ3_QandA_Test_Data_Joined.csv
                ├── 📄 LLAMA_Responses_RQ3_SA_Test_Data_Joined.csv
                ├── 📄 LLAMA_Responses_RQ3_TD_Test_Data_Joined.csv
            ├── 📁 MISTRAL
                ├── 📁 Results
                    ├── 📄 ASR_Result_MISTRAL_Responses_RQ3_QandA_Test_Data_Joined.csv
                    ├── 📄 ASR_Result_MISTRAL_Responses_RQ3_QandA_Test_Data_Joined.csv
                    ├── 📄 ASR_Result_MISTRAL_Responses_RQ3_TD_Test_Data_Joined.csv.csv
                    ├── 📄 Result_MISTRAL_Responses_RQ3_SA_Test_Data_Joined.csv
                    ├── 📄 Result_MISTRAL_Responses_RQ3_TD_Test_Data_Joined.csv
                    ├── 📄 Stats_Result_MISTRAL_Responses_RQ3_QandA_Test_Data_Joined.csv
                    ├── 📄 Stats_Result_MISTRAL_Responses_RQ3_SA_Test_Data_Joined.csv
                    ├── 📄 Stats_Result_MISTRAL_Responses_RQ3_TD_Test_Data_Joined.csv
                    ├── 📄 TSR_Result_MISTRAL_Responses_RQ3_QandA_Test_Data_Joined.csv
                    ├── 📄 TSR_Result_MISTRAL_Responses_RQ3_SA_Test_Data_Joined.csv
                    ├── 📄 TSR_Result_MISTRAL_Responses_RQ3_TD_Test_Data_Joined.csv
                ├── 📄 MISTRAL_Responses_RQ3_QandA_Test_Data_Joined.csv
                ├── 📄 MISTRAL_Responses_RQ3_SA_Test_Data_Joined.csv
                ├── 📄 MISTRAL_Responses_RQ3_TD_Test_Data_Joined.csv
            ├── 📄 RQ3_Results_GPT4o_Responses_RQ3_QandA_Test_Data_Joined.csv
            ├── 📄 RQ3_Results_GPT4o_Responses_RQ3_SA_Test_Data_Joined.csv
            ├── 📄 RQ3_Results_GPT4o_Responses_RQ3_TD_Test_Data_Joined.csv
            ├── 📄 RQ3_Results_LLAMA_Responses_RQ3_QandA_Test_Data_Joined.csv
            ├── 📄 RQ3_Results_LLAMA_Responses_RQ3_SA_Test_Data_Joined.csv
            ├── 📄 RQ3_Results_LLAMA_Responses_RQ3_TD_Test_Data_Joined.csv
            ├── 📄 RQ3_Results_MISTRAL_Responses_RQ3_QandA_Test_Data_Joined.csv
            ├── 📄 RQ3_Results_MISTRAL_Responses_RQ3_SA_Test_Data_Joined.csv
            ├── 📄 RQ3_Results_MISTRAL_Responses_RQ3_TD_Test_Data_Joined.csv
        ├── 📄 README.md
        ├── 📄 RQ3_All_Test_Data.csv
        ├── 📄 RQ3_All_Test_Data_Joined.csv
        ├── 📄 RQ3_QandA_Test_Data.csv
        ├── 📄 RQ3_SA_Test_Data.csv
        ├── 📄 RQ3_TD_Test_Data.csv
    ├── 📄 Experiments_ResearchQuestions.ipynb
    ├── 📄 README.md
├── 📄 README.md
```


## Note
Each folder and subfolder includes a dedicated **README** file with specific instructions on how to run and use the components within the package.
