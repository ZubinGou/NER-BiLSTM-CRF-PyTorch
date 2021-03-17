# NER-BiLSTM-CRF-PyTorch
PyTorch implementation of a BiLSTM-CRF model for named entity recognition.

## Requirements
- Python 3
- PyTorch 1.x

## Papers
- Bidirectional LSTM-CRF Models for Sequence Tagging (Huang et. al., 2015)
  - the first paper apply BiLSTM-CRF to NER
- Neural Architectures for Named Entity Recognition (Lample et. al., 2016)
  - pre-trained word embedding（skip-n-gram）with character-based word embeddings，improved the performance by introducing character-level features.
  > 90.94 in CoNLL 2003 (English) & 91.47 in CoNLL++
- End-to-end Sequence Labeling via Bi-directional LSTM-CNNs-CRF (Ma et al., 2016)
    - CNNs

## Dataset
- CoNLL 2003 (English)

### Evaluation
- conlleval: Perl script used to calculate FB1 (**phrase level**)

## Model
- Embeddings
    - 100d pre-trained word embedding with Glove
    - 25d charactor embedding trained by CNNs (Ma et al., 2016)
- BiLSTM-CRF (Lample et. al., 2016)

## Results
Trained with Tesla T4 for for one night (70 epochs), obtain 91.01% F1.

![](images/result.png)

## Future Works
- Next paper：
  - BiLSTM-CRF+ELMo ((Peters et al., 2018)
  - LM-LSTM-CRF (Liu et al., 2018)
  - Flair
  - ...
- 中文 NER

## References
- https://pytorch.org/tutorials/beginner/nlp/advanced_tutorial.html
- https://github.com/ZhixiuYe/NER-pytorch