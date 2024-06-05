# semantic-plausibility

This repository contains the code for the Semantic Plausibility Seminar.

## Dataset Analysis

### How to run the code

1. Clone the repository

```bash
git clone https://github.com/arshandalili/semantic-plausibility.git
cd semantic-plausibility
```

2. Create a virtual environment

The python version used in this project is 3.12.3. Please make sure you have this version installed.

You can create a virtual environment with the following commands:

```bash
python3 -m venv venv
source venv/bin/activate
```

3. Install the requirements

```bash
pip install -r requirements.txt
```

Since the dataset is not large, they are included in the repository. So there is no need to download/move any dataset. They are already in the `data` folder. (SHROOM and Concreteness dataset)

4. Run the code

Simply run the `dataset_analysis.ipynb` notebook to see the analysis of the dataset. 

Make sure to run the notebook in the virtual environment. Also, make sure that you run the first cells until the `Analysing the dataset with its characteristics` section. Then, you can simply run the characteristics you want to see.

Codes are commented and there are explanations in the notebook. If a cell takes too long or there is a need to use GPU, it is mentioned in that section.

And that's it! You can now see the analysis of the dataset! 😃
