# Analysis & Segmentation of Natural Catastrophe Events

## Definition of Nat-Cat Event

A **"nat cat event"** refers to a **natural catastrophe event** — significant natural events that cause substantial damage and disruption.

Examples include:

- Earthquakes  
- Hurricanes  
- Tornadoes  
- Floods  
- Wildfires  
- Tsunamis  
- Volcanic eruptions  

These events often result in significant economic losses, property damage, and can have severe impacts on human life and the environment.

---

## Part 1

### Task 1: Exploratory Data Analysis (EDA)

- Perform an initial inspection to understand the structure and content of the dataset.
- Provide a summary of the dataset, including:
  - Total number of articles
  - Range of publication dates
  - Basic structure of the data
  - Average length of titles
  - Presence and distribution of missing data

---

### Task 2: Title Cleaning and Relevance Filtering

- **Focus:** Analysis of the article titles
- **Challenges:** Dataset is extremely noisy; many titles are irrelevant
- **General Cleaning & Preparation:**
  - Remove duplicates
  - Trim extra whitespace
  - Strip out special characters
- **Relevance Criteria for Titles:**
  - Must **contain a location**
  - Must **represent an actual natural catastrophe event that has occurred**

---

## Part 2: Event Categorization

Develop a component that utilizes the cleaned data from **Part 1** to classify each relevant article title into one of the following five natural catastrophe categories:

1. Earthquake  
2. Flood  
3. Volcano  
4. Tornado  
5. Wildfire  

---

## Usage

- Use pip to install requirements to your terminal
- Change `config.yaml` to suit your hardware specifications and pick models:
    - `use_available_gpus`: Opt in or out of using your PC's GPU. Will only matter if a GPU is available to you.

Applicable to GPU Users:
    - `batch_size_gpu`: The batch size for GPU tasks
    - `ner_pipeline_gpu`: The Named Entity Recognition pipeline to use for GPU tasks
    - `zero_shot_model_gpu`: The Hugging Face NLI Zero-Shot-Classification for GPU tasks

Applicable to CPU Users:
    - `batch_size_cpu`: The batch size for GPU tasks
    - `ner_pipeline_cpu`: The Named Entity Recognition pipeline to use for GPU tasks
    - `zero_shot_model_cpu`: The Hugging Face NLI Zero-Shot-Classification for GPU tasks

Available NER Pipelines: https://spacy.io/models/en#benchmarks. 'en_core_web_sm' CPU compatible & quick. 'en_core_web_trf' GPU compatible, more accurate but slow.

Availble Hugging Face Models: https://huggingface.co/models?pipeline_tag=zero-shot-classification

Run notebooks in order:

1. 1_Exploratory_Data_Analysis.ipynb
2. 2_DataCleaning.ipynb
3. 3_Data_Segmentation.ipynb