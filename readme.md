<h3 align="center">FinancialPressAnalysisBERT</h3>

---

[Wissem Chabchoub](https://www.linkedin.com/in/wissem-chabchoub/) | [Contact us](chb.wissem@gmail.com)

## 📝 Table of Contents

- [📝 Table of Contents](#-table-of-contents)
- [🧐 About <a name = "about"></a>](#-about)
- [🎥 Repository Structure  <a name = "repo-struct"></a>](#-repository-structure)


## 🧐 About <a name = "about"></a>

In this project, we are scrapping artciles from Reuters Website discussing specific assets from the american market. We then will use a version of BERT called FinBERT (https://arxiv.org/abs/2006.08097) to analyse the sentiment (positive, negative, neutral) oh these articles. The sentiment analysis is carried on sentence wise. We then apply a simple convolution vector before averaging the sentiments for each article.
This appraoch can be generalized to every other market and every othe asset or ticker. 

Please download FinBERT and place it in FinBERT folder:
* [Sentiment analysis model trained on Financial PhraseBank](https://prosus-public.s3-eu-west-1.amazonaws.com/finbert/finbert-sentiment/pytorch_model.bin)

## 🎥 Repository Structure  <a name = "repo-struct"></a>


1. `data`: Where the input tickers are saved and the scrapped articles and their features will be saved
2. `FinBERT`: Where the language model is saved
3. `fetchers`: Contains the main python class
4. `env` : contains the docker env
5. `Notebook.ipynb` : a jupyter notebook for running and testing
