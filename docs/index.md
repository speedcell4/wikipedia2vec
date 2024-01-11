# Wikipedia2Vec

---

<a class="github-button" href="https://github.com/wikipedia2vec/wikipedia2vec" data-size="large" data-show-count="true" aria-label="Star wikipedia2vec/wikipedia2vec on GitHub">Star</a>

## Introduction

Wikipedia2Vec is a tool used for obtaining embeddings (or vector representations) of words and entities (i.e., concepts that have corresponding pages in Wikipedia) from Wikipedia.
It is developed and maintained by [Studio Ousia](http://www.ousia.jp).

This tool enables you to learn embeddings of words and entities simultaneously, and places similar words and entities close to one another in a continuous vector space.
Embeddings can be easily trained by a single command with a publicly available Wikipedia dump as input.

This tool implements the [conventional skip-gram model](https://en.wikipedia.org/wiki/Word2vec) to learn the embeddings of words, and its extension proposed in [Yamada et al. (2016)](https://arxiv.org/abs/1601.01343) to learn the embeddings of entities.

An empirical comparison between Wikipedia2Vec and existing embedding tools (i.e., FastText, Gensim, RDF2Vec, and Wiki2vec) is available [here](https://arxiv.org/abs/1812.06280).

## Pretrained Embeddings

Pretrained embeddings for 12 languages (i.e., English, Arabic, Chinese, Dutch, French, German, Italian, Japanese, Polish, Portuguese, Russian, and Spanish) can be downloaded from [this page](pretrained.md).

## Use Cases

Wikipedia2Vec has been applied to the following tasks:

- Entity linking: [Yamada et al., 2016](https://arxiv.org/abs/1601.01343), [Eshel et al., 2017](https://arxiv.org/abs/1706.09147), [Chen et al., 2019](https://arxiv.org/abs/1911.03834), [Poerner et al., 2020](https://arxiv.org/abs/1911.03681), [van Hulst et al., 2020](https://arxiv.org/abs/2006.01969).
- Named entity recognition: [Sato et al., 2017](http://www.aclweb.org/anthology/I17-2017), [Lara-Clares and Garcia-Serrano, 2019](http://ceur-ws.org/Vol-2421/eHealth-KD_paper_6.pdf).
- Question answering: [Yamada et al., 2017](https://arxiv.org/abs/1803.08652), [Poerner et al., 2020](https://arxiv.org/abs/1911.03681).
- Entity typing: [Yamada et al., 2018](https://arxiv.org/abs/1806.02960).
- Text classification: [Yamada et al., 2018](https://arxiv.org/abs/1806.02960), [Yamada and Shindo, 2019](https://arxiv.org/abs/1909.01259), [Alam et al., 2020](https://link.springer.com/chapter/10.1007/978-3-030-61244-3_9).
- Relation classification: [Poerner et al., 2020](https://arxiv.org/abs/1911.03681).
- Paraphrase detection: [Duong et al., 2018](https://ieeexplore.ieee.org/abstract/document/8606845).
- Knowledge graph completion: [Shah et al., 2019](https://aaai.org/ojs/index.php/AAAI/article/view/4162), [Shah et al., 2020](https://www.aclweb.org/anthology/2020.textgraphs-1.9/).
- Fake news detection: [Singh et al., 2019](https://arxiv.org/abs/1906.11126), [Ghosal et al., 2020](https://arxiv.org/abs/2010.10836).
- Plot analysis of movies: [Papalampidi et al., 2019](https://arxiv.org/abs/1908.10328).
- Novel entity discovery: [Zhang et al., 2020](https://arxiv.org/abs/2002.00206).
- Entity retrieval: [Gerritse et al., 2020](https://link.springer.com/chapter/10.1007%2F978-3-030-45439-5_7).
- Deepfake detection: [Zhong et al., 2020](https://arxiv.org/abs/2010.07475).
- Conversational information seeking: [Rodriguez et al., 2020](https://arxiv.org/abs/2005.00172).
- Query expansion: [Rosin et al., 2020](https://arxiv.org/abs/2012.12065).

## References

If you use Wikipedia2Vec in a scientific publication, please cite the following paper:

Ikuya Yamada, Akari Asai, Jin Sakuma, Hiroyuki Shindo, Hideaki Takeda, Yoshiyasu Takefuji, Yuji Matsumoto, [Wikipedia2Vec: An Efficient Toolkit for Learning and Visualizing the Embeddings of Words and Entities from Wikipedia](https://arxiv.org/abs/1812.06280).

```
@inproceedings{yamada2020wikipedia2vec,
  title = "{W}ikipedia2{V}ec: An Efficient Toolkit for Learning and Visualizing the Embeddings of Words and Entities from {W}ikipedia",
  author={Yamada, Ikuya and Asai, Akari and Sakuma, Jin and Shindo, Hiroyuki and Takeda, Hideaki and Takefuji, Yoshiyasu and Matsumoto, Yuji},
  booktitle = {Proceedings of the 2020 Conference on Empirical Methods in Natural Language Processing: System Demonstrations},
  year = {2020},
  publisher = {Association for Computational Linguistics},
  pages = {23--30}
}
```

The embedding model was originally proposed in the following paper:

Ikuya Yamada, Hiroyuki Shindo, Hideaki Takeda, Yoshiyasu Takefuji, [Joint Learning of the Embedding of Words and Entities for Named Entity Disambiguation](https://arxiv.org/abs/1601.01343).

```
@inproceedings{yamada2016joint,
  title={Joint Learning of the Embedding of Words and Entities for Named Entity Disambiguation},
  author={Yamada, Ikuya and Shindo, Hiroyuki and Takeda, Hideaki and Takefuji, Yoshiyasu},
  booktitle={Proceedings of The 20th SIGNLL Conference on Computational Natural Language Learning},
  year={2016},
  publisher={Association for Computational Linguistics},
  pages={250--259}
}
```

The text classification model implemented in [this example](https://github.com/wikipedia2vec/wikipedia2vec/tree/master/examples/text_classification) was proposed in the following paper:

Ikuya Yamada, Hiroyuki Shindo, [Neural Attentive Bag-of-Entities Model for Text Classification](https://arxiv.org/abs/1909.01259).

```
@article{yamada2019neural,
  title={Neural Attentive Bag-of-Entities Model for Text Classification},
  author={Yamada, Ikuya and Shindo, Hiroyuki},
  booktitle={Proceedings of The 23th SIGNLL Conference on Computational Natural Language Learning},
  year={2019},
  publisher={Association for Computational Linguistics},
  pages = {563--573}
}
```

## License

[Apache License 2.0](http://www.apache.org/licenses/LICENSE-2.0)
