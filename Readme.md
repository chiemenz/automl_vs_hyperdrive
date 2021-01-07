
## Citations & Required Downloads

### Download A - Polarity Dictionaries
> **Please note that part of the pre-processing involves sentiment polarity dictionaries which were created by:**
> 
> _William L. Hamilton, Kevin Clark, Jure Leskovec, and Dan Jurafsky_
> _Inducing Domain-Specific Sentiment Lexicons from Unlabeled Corpora. ArXiv preprint (arxiv:1606.02820). 2016._ 
>
> Download the sentiment polarity dictionaries via:
>
> [Sentiment scores for frequent words](https://nlp.stanford.edu/projects/socialsent/files/socialsent_hist_freq.zip)
>
> [Sentiment scores for adjectives](https://nlp.stanford.edu/projects/socialsent/files/socialsent_hist_adj.zip)
>
####Save the unzipped files in the polarity directory to get the following structure:
```
automl_vs_hyperdrive/
│
└── data/
  └── polarity_data
            ├── socialsent_hist_adj 
            │      └── adjectives
            │            └── * many_tsv_files
            │
            └── socialsent_hist_freq
                   └── frequent_words
                         └── * many_tsv_files
```

### Download B - Dataset
> Please note that the modeling is based on the **Kaggle Trip Advisor Reviews Dataset** see citation bellow
> 
> _Alam, M. H., Ryu, W.-J., Lee, S., 2016. Joint multi-grain topic sentiment: modeling semantic aspects for online reviews. Information Sciences 339, 206–223._
> 
> [Kaggle Trip Advisor Reviews](https://www.kaggle.com/andrewmvd/trip-advisor-hotel-reviews)
####Save the unzipped files in the polarity directory to get the following structure:
```
automl_vs_hyperdrive/
│
└── data/
  └── datasets
            └── socialsent_hist_adj 
            │      └── adjectives
            │            └── * many_tsv_files
            │
            └── socialsent_hist_freq
                   └── frequent_words
                         └── * many_tsv_files
```


## Repository setup


* I. Create a virtual environment

```
conda create --name automl_vs_hyperdrive python=3.7
```
* II. Activate your conda environment
```
activate automl_vs_hyperdrive
```
* III. Install requirements.txt
```
pip install -r requirements.txt
```
* IV. Execute setup.py 
```
python setup.py develop
```
* V. Download  _en_trf_robertabase_lg_ spacy model
```
python -m spacy download en_trf_robertabase_lg
```
* VI. Download _en_core_web_md_ spacy model
```
python -m spacy download en_core_web_md
```