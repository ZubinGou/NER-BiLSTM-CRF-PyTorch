# NER-BiLSTM-CRF-PyTorch
PyTorch implementation of a BiLSTM-CRF model for named entity recognition.

## Paper
- Bidirectional LSTM-CRF Models for Sequence Tagging (Huang et. al., 2015)
  - 首次将BiLSTM-CRF用于序列标注
- Neural Architectures for Named Entity Recognition (Lample et. al., 2016)
  - 最大特点是在pre-trained word embedding（skip-n-gram）的基础上结合了character-based word embeddings，通过引入字符级特征提高了模型在NER任务中的表现
    - 90.94 in CoNLL 2003 (English)
    - 91.47 in CoNLL++

## Related Works
- Bidirectional LSTM-CRF models for sequence tagging


## Corpus
- [ ] CoNLL 2003 (English)
- [ ] CoNLL++

## Future Works
- 后续paper：
  - BiLSTM-CNN-CRF (Ma et al., 2016)
  - BiLSTM-CRF+ELMo ((Peters et al., 2018)
  - LM-LSTM-CRF (Liu et al., 2018)
  - Flair
  - ...
- 中文NER

## References
- https://pytorch.org/tutorials/beginner/nlp/advanced_tutorial.html