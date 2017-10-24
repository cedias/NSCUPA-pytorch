# HAN-UPA-pytorch
Pytorch implementation of Neural Sentiment Classification with User &amp; Product Attention paper: https://aclweb.org/anthology/D16-1171

#Requirements
- Pytorch (>= 0.2)
- Spacy (for tokenizing)
- Gensim (for building word vectors)
- tqdm (for fancy graphics)

#Scripts:
- `minimal_ex(_cuda).sh` quick start scripts that does everything and starts learning (just `chmod +x` them).
- `prepare_data.py` transforms gzip files as found on [Julian McAuley Amazon product data page](http://jmcauley.ucsd.edu/data/amazon/) to lists of `(user,item,review,rating)` tuples and builds word vectors if `--create-emb` option is specified.
- `main.py` trains a Hierarchical Model.
- `Data.py` holds data managing objects.
- `Nets.py` holds networks.
- `beer2json.py` is an helper script if you happen to have the ratebeer/beeradvocate datasets.
