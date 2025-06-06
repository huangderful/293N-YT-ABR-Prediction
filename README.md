# 293N-YT-ABR-Prediction
This repository trains models on adaptive bitrate (ABR) decisions using the Requet and Puffer Dataset and interprets model behavior using Trustee and AQUA.

## Setup
Create a virtual environment and install requirements.txt (**Python 3.11.11** is recommended).
```
pip install -r requirements.txt
```

## Running the Requet Pipeline
1. Clone the [RequetDataSet](https://github.com/Wimnet/RequetDataSet) repository.

2. Run `preprocess.py` to create CSV files from the Requet data set.

3. Run `requet_pipeline.ipynb` to train a Random Forest model and generate Trustee and Aqua explanations.


## Running the Puffer Pipeline
1. Download the [Puffer data](https://puffer.stanford.edu/results/2019-01-26/) for video_sent and client_buffer. The exact files we used are linked here: https://drive.google.com/file/d/1yTxNgZ5huNfH3peBRAkXiSDEptG5p7dH/view?usp=sharing

2. Place the downloaded CSV files into the appropriate subdirectories inside `/puffer_tests`.

3. Run the `expt_split.ipynb` notebook to preprocess and split the data.

4. Run `puffer_pipeline.ipynb` to train models and generate the TRUSTEE and AQUA reports.
