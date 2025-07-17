# Results Attack Success Rate (ASR)

This folder contains all results for the ASR metrics, as well as two folders (GPT4o and LLAM) with the individual results

## Structure
```
Experiments/RQ3/Results/
├── LLAMA/                      
│   └── ...   
├── GPT4o/                      
│   └── ...  
│ ├── RQ3_Results_GPT4o_Responses_RQ3_QandA_Test_Data_Joined.csv
│ ├── RQ3_Results_GPT4o_Responses_RQ3_SA_Test_Data_Joined.csv
│ ├── RQ3_Results_GPT4o_Responses_RQ3_TD_Test_Data_Joined.csv
│ ├── RQ3_Results_LLAMA_Responses_RQ3_QandA_Test_Data_Joined.csv
│ ├── RQ3_Results_LLAMA_Responses_RQ3_SA_Test_Data_Joined.csv
│ └── RQ3_Results_LLAMA_Responses_RQ3_TD_Test_Data_Joined.csv

## Contents
- **RQ3_Results_GPT4o_Responses_RQ3_QandA_Test_Data_Joined.csv** - ASR values for the Question & Answering intent using GPT4o.

- **RQ3_Results_GPT4o_Responses_RQ3_SA_Test_Data_Joined.csv**  - ASR values for the Sentiment Analysis intent using GPT4o.

- **RQ3_Results_GPT4o_Responses_RQ3_TD_Test_Data_Joined.csv**  - ASR values for the Toxicity Detection intent using GPT4o.

- **RQ3_Results_LLAMA_Responses_RQ3_QandA_Test_Data_Joined.csv**  - ASR values for the Question & Answering intent using LLaMA.

- **RQ3_Results_LLAMA_Responses_RQ3_SA_Test_Data_Joined.csv** - ASR values for the Sentiment Analysis intent using LLaMA.

- **RQ3_Results_LLAMA_Responses_RQ3_TD_Test_Data_Joined.csv** - ASR values for the Toxicity Detection intent using LLaMA.

## GPT4o Folder
  Contains additional analyses specific to GPT4o experiments.
## LLaMa2 Folder
  Contains additional analyses specific to LLaMa experiments.
