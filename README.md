# 293N-YT-ABR-Prediction
1. setup a venv and install requirements.txt (I used python 3.12.10)
2. Run preprocess.py ==> Creates csvs from the Requet DataSet which is taken from https://github.com/gao-keyong/requet/
- The RequetDataSet folder is the same as the repo and you need to clone this into your branch cuz i gitignored it: https://github.com/Wimnet/RequetDataSet

3. Run the jupyter notebook `requet_trustee_pipeline.ipynb` which trains an RF and uses trustee https://github.com/TrusteeML/trustee


---
To run the pipeline
1. Go on puffer and download video sent, client buffer, and ssim csvs (not all days require client buffer but my code assumes it is needed)

All code runs for this date:
https://puffer.stanford.edu/results/2019-01-26/

2. Run expt_split
3. Now you can run the COMPLETE_PIPELINE.ipynb for both TRUSTEE and AQUA reports

