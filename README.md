# semantic-plausibility

This repository contains the code for the Semantic Plausibility Seminar.

## How to run the code

1. Clone the repository

```bash
git clone https://github.com/arshandalili/semantic-plausibility.git
cd semantic-plausibility
```

2. Create a virtual environment

The python version used in this project is `3.12.3`. Please make sure you have this version installed.

You can create a virtual environment with the following commands:

```bash
python3 -m venv venv
source venv/bin/activate
```

3. Install the requirements

```bash
pip install -r requirements.txt
```

## Dataset Analysis

Since the dataset is not large, they are included in the repository. So there is no need to download/move any dataset. They are already in the `data` folder. (SHROOM and Concreteness dataset)

4. Run the code

Simply run the `dataset_analysis.ipynb` notebook to see the analysis of the dataset. 

Make sure to run the notebook in the virtual environment. Also, make sure that you run the first cells until the `Analysing the dataset with its characteristics` section. Then, you can simply run the characteristics you want to see.

Codes are commented and there are explanations in the notebook. If a cell takes too long or there is a need to use GPU, it is mentioned in that section.

And that's it! You can now see the analysis of the dataset! 😃

## Models

There are three models that are implemented in this repository. They are:

1. SentenceBERT
2. UniEval
3. Fine-tuned LLM (Llama 3)

Each model has its own folder with its own related files. Note that you might need to install some additional libraries to run the models. But don't worry! Below are the instructions on how to run each model.

### SentenceBERT

Make sure that you have the files in the following structure:

![Screenshot 2024-07-05 at 2 17 15 PM](https://github.com/arshandalili/semantic-plausibility/assets/57400500/d6ea68a7-9518-4037-82ce-f3260a392495)

Then, you can run the `SentenceBERT.ipynb` notebook to see the results of the model. Make sure to run all the cells in the notebook in order to see the results.

### UniEval

Make sure that you have the files in the following structure:

![Screenshot 2024-07-05 at 3 33 22 PM](https://github.com/arshandalili/semantic-plausibility/assets/57400500/cee053af-f4c4-4511-8d8d-9c1c89813062)

Then, you can run the `UniEval.ipynb` notebook to see the results of the model. Please note that you need to run all the cells in the notebook. The first cells are the one that will install the UniEval library. It is better to run this notebook in an environment with GPU.

### Fine-tuned LLM (Llama 3)

Due to the complexity of the model, let's divide the instructions into two parts:

#### Fine-tuning the model

Make sure that you have the files in the following structure (especially `data` folder and `train.csv`) and set up the environment below:

![Screenshot 2024-07-05 at 3 02 36 PM](https://github.com/arshandalili/semantic-plausibility/assets/57400500/e8eefd30-c3b2-4940-b23b-2b74f2fc3bf5)

![Screenshot 2024-07-05 at 3 28 31 PM](https://github.com/arshandalili/semantic-plausibility/assets/57400500/ff59f74c-3496-403a-ae62-0f389a652d11)

My suggestion is to run the model in Kaggle with a dataset and its notebook there. Due to the complexity of the task, let me know if you need any help with this.

But, just FYI, I made the prompts by running the `Prompt.ipynb` notebook. This will create the prompts for fine-tuning the model.
For next steps, please refer to the `LLM_Finetune.ipynb` notebook to see more details on how to run the model.


#### Running the model (Inference)

For the inference part, you should run the `Installing and importing requirements` part first and then run the `Inference` part of the `LLM_Finetune.ipynb` notebook. Basically, you need to omit the `Fine-tune LLM` part.


### Ensemble (Majority Voting)

To see the results of the ensemble model, you can run the `Ensemble_and_Results.ipynb` notebook in the `models/Ensemble_and_Results/` folder. This notebook will show the results of the models themselves plus their majority voting for all tasks and overall.

And that's it! You can now run and see the results of the models! 😃