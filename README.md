# Synthetic-data-for-aggregated-prosumers
This repository contains the synthetic datasets generated and used in the study presented in the manuscript “Calibrated Uncertainty Quantification for Prosumer Flexibility Aggregation in Ancillary Service Markets,” supporting transparency and reproducibility of the results. Please find preprint at:
https://arxiv.org/abs/2601.14663 for details and context.

## Repository Structure
├── Business_model_test_data.zip
├── LICENSE
├── MCD_CP_training_data.zip
└── README.md


### MCD_CP_training_data.zip

**Purpose:**  
This data was used to train the proposed hybrid MCD-CP framework for predicting flexibility, using the methodology presented in Section 4. Mathematical notation used for this set was $\mathcal{D}$ in the manuscript.

**After extraction:**
MCD_CP_training_data/
├── MCD_CP_training_data.csv

**Data characteristics:**

- **Format:** CSV  
- **Time resolution:** hourly, each hour is treated as a separate column
- **Data structure:** Structured such that each row contains input and output pair for training or infering from an ML model  
- For detailed descriptions of each column, input and output sets refer to the manuscript

### Business_model_test_dataset.zip

**Purpose:**  
This data was used to evaluate the aggregator's business model and produce the results in Section 5.2. Mathematical notation used for this set was $\mathcal{D}_{\beta}$ in the manuscript.

**After extraction:**
Business_model_test_dataset/
├── Business_model_test_dataset.csv

- **Format:** CSV  
- **Time resolution:** hourly, each hour is treated as a separate column
- **Data structure:** Structured such that each row contains input and output pair for infering from an ML model. Key filters such as case number and incentive factor are added to the dataset  
- For detailed descriptions of each column, input and output sets refer to the manuscript

## Usage Instructions

1. Download the `.zip` archives
2. Extract them to desired location
3. Load csv using preferred software. Recommended to use Pandas dataframe in python.    

## Reproducibility
These datasets are provided to enable reproduction of the results reported in the associated study.
Refer to the manuscript for detailed methodology and data usage within the optimisation and/or machine learning framework. 

Please refer to the LICENSE file for information on licensing and permitted use. If you use this dataset in your work, please cite the associated manuscript available at:
https://arxiv.org/abs/2601.14663
