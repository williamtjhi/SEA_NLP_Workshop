# SEA_NLP_Workshop

This is a repo containing the files needed to run all the demos for the SEA NLP track of the AIP Developer Conference 2022. Please read and follow the instructions below to run the demo Notebooks. We will go through the demos together during the session. There is also a separate deck of slides that will accompany the demo. This deck will be sent to the organiser of the conference after the session. 

## Steps needed before running the demo Notebooks
1. Clone this repo
2. Go to the repo folder in your local directory
3. Copy some large files as follows:
   - Download to the `models` folder, the IndoBERT model fine-tuned for Indonesian NER [here](https://drive.google.com/file/d/1PUEVO9Yd69p_p2lQyNwmJFKJSgHnr7-i/view?usp=sharing)
   - Download to the `Datasets/IMDB` folder, the [training set of the IMDB dataset](https://drive.google.com/file/d/1Pc-3u6CUBqvcQcsZKzCBaLZYKjDAN8EQ/view?usp=sharing)
   - Download to the `Resources` folder, the `fasttext` [English embedding binary](https://dl.fbaipublicfiles.com/fasttext/vectors-crawl/cc.en.300.bin.gz). This is a huge file and it will take a while to download. Unzip the file after download: `gunzip -d cc.en.300.bin.gz`.
   - Download to the `Resources` folder, the `fasttext` [Indonesian embedding binary](https://dl.fbaipublicfiles.com/fasttext/vectors-crawl/cc.id.300.bin.gz). This is a huge file and it will take a while to download. Unzip the file after download: `gunzip -d cc.id.300.bin.gz`.
4. To run most of the demo Notebooks (except `IndoBERT_NER.ipynb`, which needs a separate environment), do the following:
   - Create a new environment `sea_nlp1` (you can use any other name of your preference for your environment): `conda create --name sea_nlp1 python=3.7`
   - Go to the new environment: `conda activate sea_nlp1`
   - Install the dependencies: `pip install -r requirements.txt`
   - Start Jupyter: `jupyter notebook`
   - Open one of the Notebooks (e.g. `SentimentAnalysis_EN_2.ipynb`) in your browser to run the demo
5. To run the demo Notebooks: `IndoBERT_NER.ipynb`, which depends on an older version of `transformers`, do the following:
   - Exit from any environment you are in
   - Create a new environment `sea_nlp2` (you can use any other name of your preference for your environment): `conda create --name sea_nlp2 python=3.7`
   - Go to the new environment: `conda activate sea_nlp2`
   - Install the dependencies: `pip install -r requirements_IndoBERT.txt`
   - Start Jupyter: `jupyter notebook`
   - Open the Notebook `IndoBERT_NER.ipynb` in your browser to run the demo
   
