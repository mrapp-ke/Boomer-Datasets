# README

This repository contains a selection of real-world benchmark datasets for [multi-label classification](https://en.wikipedia.org/wiki/Multi-label_classification). They are provided in the [Mulan data format](http://mulan.sourceforge.net/format.html) and originate from the publicly available collections of datasets that are provided by the following projects:

* The [MEKA](https://waikato.github.io/meka/datasets) project
* The [MULAN](http://mulan.sourceforge.net/datasets-mlc.html) project
* The [LIBSVM](https://www.csie.ntu.edu.tw/~cjlin/libsvmtools/datasets) project
* The [MLDA](https://www.uco.es/kdis/mllresources) tool for analyzing multi-label datasets

The datasets are intended for use with the [BOOMER](https://github.com/mrapp-ke/Boomer) machine learning algorithm and have been used for empirical studies that are concerned with this particular multi-label classification method.

In addition, this repositories does also include [toy datasets](https://github.com/mrapp-ke/Boomer-Datasets/tree/main/toy-datasets) that are well-suited for debugging purposes due to their small size and may be useful to analyze the behavior of learning algorithms.

Moreover, this repository does also contain several [synthetic datasets](https://github.com/mrapp-ke/Boomer-Datasets/tree/main/synthetic-datasets) with varying characteristics, as well as a Python script for generating them, originating from [this](https://link.springer.com/content/pdf/10.1007/s10994-012-5285-8.pdf) paper. These datasets may be useful to investigate the ability of different classification methods to deal with conditional and marginal label dependence. The motivation to capture hidden dependencies between labels that can be found in most real-world datasets is a driving force of research on multi-label classification.

## Cloning the Repository

This repository uses [Git Large File Storage (LFS)](https://git-lfs.github.com/). It is required to have this open source extension to the Git version control system installed on your computer. Once you have installed the software, the repository can be cloned as usual via the following command:

```
git clone https://github.com/mrapp-ke/Boomer-Datasets.git
```

## Benchmark Datasets

In accordance with the [Mulan data format](http://mulan.sourceforge.net/format.html), all datasets that are provided by this repository come as an [.arff](http://weka.wikispaces.com/ARFF) file that specify the feature values and ground truth labels of the examples they entail. In addition, a .xml file that specifies the names of the available labels is provided for each dataset. In most cases, predefined splits of a dataset into training and test data (indicated by including the suffixes `-train` and `-test` in the respective file names) are available as well.

In the following, we provide a description of the datasets that are included in this repository, as well as references to the original authors:

#### 20NG

*K. Lang. 2008. The 20 newsgroup dataset. http://people.csail.mit.edu/jrennie/20Newsgroups/.*

A compilation of around 20,000 newsgroup posts on 20 different topics.

#### Bibtex

*Ioannis Katakis, Grigorios Tsoumakas, and Ioannis Vlahavas. Multilabel Text Classification for Automated Tag Suggestion. In Proceedings of the ECML/PKDD 2008 Discovery Challenge, 2008.*

A dataset that is based on the ECML/PKDD 2008 discovery challenge. It contains 7395 Bibtex entries from the BibSonomy social bookmark and publication sharing system, annotated with a subset of the tags that have been assigned by BibSonomy users.

#### Birds

*Forrest Briggs et al. The 9th annual MLSP competition: New methods for acoustic classification of multiple simultaneous bird species in a noisy environment. In IEEE International Workshop on Machine Learning for Signal Processing, pp. 1–8, 2013.*

A dataset that is aimed at predicting the set of bird species that one can hear in ten-second audio clips.

#### Bookmarks

*Ioannis Katakis, Grigorios Tsoumakas, and Ioannis Vlahavas. Multilabel Text Classification for Automated Tag Suggestion. In Proceedings of the ECML/PKDD 2008 Discovery Challenge, 2008.*

A dataset that is based on the ECML/PKDD 2008 discovery challenge. It contains bookmark entries from the BibSonomy social bookmark and publication sharing system.

#### CAL500

*Douglas Turnbull, Luke Barrington, David Torres and Gert Lanckriet. Semantic Annotation and Retrieval of Music and Sound Effects, IEEE Transactions on Audio, Speech and Language Processing 16(2), pp. 467-476, 2008.*

A music dataset that is composed of 502 songs. Each one was manually annotated with a subset of 174 tags that correspond to 6 semantic concepts: instrumentation, vocal characteristics, genres, emotions, acoustic quality and usage terms.

#### Corel5k

*Pinar Duygulu, Kobus Barnard, Nando de Freitas, and David Forsyth, Object recognition as machine translation: Learning a lexicon for a fixed image vocabulary , 7th European Conference on Computer Vision, pp. 97-112, 2002.*

An popular benchmark dataset for image classification that is based on 5,000 Corel images.

#### Delicious

*G. Tsoumakas, I. Katakis, and I. Vlahavas. Effective and Efficient Multilabel Classification in Domains with Large Number of Labels. In Proc. ECML/PKDD 2008 Workshop on Mining Multidimensional Data, 2008.*

A dataset that contains the textual data of web pages, together with corresponding tags.

#### Emotions

*G. Tsoumakas, I. Katakis, and I. Vlahavas. Effective and Efficient Multilabel Classification in Domains with Large Number of Labels. In Proc. ECML/PKDD 2008 Workshop on Mining Multidimensional Data, 2008.*

A small dataset that is aimed at classifying music into emotions, based on the Tellegen-Watson-Clark model of mood.

#### Enron

*Jesse Read, Bernhard Pfahringer, and Geoff Holmes. Multi-label Classification Using Ensembles of Pruned Sets. In Proceedings of the 2008 Eighth IEEE International Conference on Data Mining, pp. 995–1000, 2008.*

This datasets includes a subset of the Enron e-mail corpus, annotated with different topical categories.

#### Eukaryote-GO and Eukaryote-Pse-AAC

*Jianhua Xu, Jiali Liu, Jing Yin, and Chengyu Sun. A multi-label feature extraction algorithm via maximizing feature variance and feature-label dependence simultaneously. Knowledge-Based Systems, 98: pp. 172 — 184, 2016*

A dataset from the field of biology that is used to predict the sub-cellular locations of proteins according to 7,766 sequences for the Eukaryote species. Two variants that come with gene onology feature (GO) or include 20 amino acid, 20 pseudo-amino acid and 400 diptide components (Pse-AAC) are available.

#### EUR-Lex-DC, EUR-Lex-EV and EUR-Lex-SM

*Eneldo Loza Mencía and Johannes Fürnkranz. Efficient Pairwise Multilabel Classification for Large-Scale Problems in the Legal Domain. In Proceedings of the European Conference on Machine Learning and Principles and Practice of Knowledge Disocvery in Databases (ECML-PKDD-2008), pp. 50–65. 2008.*

A collection of 19,348 documents about European Union law. It contains many different types of documents, such as treaties or case-law and legislative proposals, which are indexed according to several orthogonal categorization schemes. The most important categorization is provided by the EUROVOC descriptors, which form a topical hierarchy with almost 4,000 categories that are concerned with different aspects of European law.

#### Flags

*E.C. Goncalves, Alexandre Plastino, and Alex A. Freitas. A genetic algorithm for optimizing the label ordering in multi-label classifier chains. In IEEE 25th International Conference on Tools with Artificial Intelligence, pp. 469–476. 2013.*

The goal of this dataset is to predict certain characteristics of flags, such as colors or shapes, based on information about the corresponding countries.

#### Foodtruck

*Adriano Rivolli, Larissa C. Parker, and Andre C.P.L.F. de Carvalho. Food Truck Recommendation Using Multi-label Classification. In EPIA 2017: Progress in Artificial Intelligence, pp. 585–596, 2017.*

A dataset that was created from a survey among 407 participants who were either approached at fast food festivals and popular events or anonymously received a request to answer a questionnaire, describing their preferences when it comes to their favorite food trucks.

#### Genbase

*Sotiris Diplaris, Grigorios Tsoumakas, Pericles Mitkas, and Ioannis Vlahavas. Protein Classification with Multiple Algorithms. In Procedings of the Panhellenic Conference on Informatics, pp. 448–456, 2005.*

A dataset for protein function classification. Each example represents a protein and each label corresponds to a protein class.

#### Image

*Min-Ling Zhang and Zhi-Hua Zhou. ML-kNN: A lazy learning approach to multi-label learning. Pattern Recognition, 40(7): pp. 2038–2048, 2007.*

An image classification dataset that is composed of 2,000 images. Each image was first converted to the CIE Luv space. Afterwards, it was divided into 49 blocks using a 7x7 grid, where in each block the first and second moments (mean and variance) of each band are computed, corresponding to a low-resolution image and computationally inexpensive texture features. Finally, each image is transformed into a 294-dimensional feature vector.

#### IMDB

*Jesse Read. Scalable multi-label classification. PhD Thesis, University of Waikato, 2010.*

This dataset contains 120,919 textual summaries of movie plots that have been obtained from the Internet Movie Database (www.imdb.com). Each summary is labeled with one or more movie genres.

#### Langlog

*Jesse Read. Scalable multi-label classification. PhD Thesis, University of Waikato, 2010.*

A dataset that was created from the Language Log Forum, where various topics related to language were discussed.

#### Mediamill

*C.G.M. Snoek, M.Worring, J.C. van Gemert, J.-M. Geusebroek, A.W.M. Smeulders. The Challenge Problem for Automated Detection of 101 Semantic Concepts in Multimedia, In Proceedings of ACM Multimedia, 421-430. 2006.*

A multimedia dataset for generic video indexing, which was extracted from the TRECVID 2005/2006 benchmark. This dataset contains 85 hours of international broadcast news data, annotated with 100 labels. Each video is represented as a 120-dimensional feature vector of numerical features.

#### Medical

*John P. Pestian, Christopher Brew, Pawel Matykiewicz, D. J. Hovermale, Neil Johnson, K. Bretonnel Cohen, and Wodzislaw Duch. A shared task involving multi-label classification of clinical free text. In Proceedings of the Workshop on BioNLP 2007: Biological, Translational, and Clinical Language Processing (BioNLP ’07), pp. 97–104, 2007.*

This dataset is based on the data that was made available during the Computational Medicine Centers 2007 Medical Natural Language Processing Challenge 10. It consists of 978 clinical text reports, labeled with one or more out of 45 disease codes.

#### Nus-Wide-cVLADplus

*Tat-Seng Chua, Jinhui Tang, Richang Hong, Haojie Li, Zhiping Luo, and Yan-Tao Zheng. “NUS-WIDE: A Real-World Web Image Database from National University of Singapore”, ACM International Conference on Image and Video Retrieval, 2009.*

An image classification dataset, where images are represented using 128-D cVLAD+ features.

#### Ohsumed

*Thorsten Joachims, Text Categorization with Support Vector Machines: Learning with Many Relevant Features. In Proceeding of the European Conference on Machine Learning (ECML), 1998.*

This dataset consists of medical abstracts from the MeSH categories of the year 1991 that should be assigned to 23 cardiovascular disease categories.

#### Reuters-K500

*Grigorios Tsoumakas and Ioannis Vlahavas. Random k-Labelsets: An Ensemble Method for Multilabel Classification. In Proceedings of the European Conference on Machine Learning (ECML), pp. 406–417, 2007.*

A well-known benchmark dataset for text classification that was created from the larger Reuters-RCV1 corpus by selecting a subset of 500 features.

#### Scene

*Matthew R. Boutell, Jiebo Luo, Xipeng Shen, and Christopher M. Brown. Learning multi-label scene classification. Pattern Recognition, 37(9): pp. 1757–1771, 2004.*

An image dataset that contains 2,407 images, annotated with up to 6 labels: beach, sunset, fall foliage, field, mountain and urban. Each image is represented by 294 visual features, corresponding to spatial color moments in the LUV space.

#### Slashdot

*Jesse Read. Scalable multi-label classification. PhD Thesis, University of Waikato, 2010.*

A dataset that consists of article blurbs with subject categories, mined from http://slashdot.org.

#### Stackex-Chemistry, Stackex-Chess, Stackex-Coffee, Stackex-Cooking, Stackex-CS, Stackex-Philosophy

*Francisco Charte and David Charte. Working with multilabel datasets in R: The MLDR package. The R Journal, 7(2):149–162, 2015.*

A collection of text classification datasets, generated from text that has been obtained from a selection of Stack Exchange forums.

#### TMC2007

*A. Srivastava, B. Zane-Ulman: Discovering recurring anomalies in text reports regarding complex space systems. In: IEEE Aerospace Conference, 2005.*

A subset of the Aviation Safety Reporting System dataset. It contains 28,596 aviation safety text reports about events that took place during a flight and that have been submitted by the flight crew afterwards. The goal is to label each document with the types of problems they describe. The dataset includes 49,060 discrete attribute that correspond to the terms that occur in the text reports. The safety reports are provided with 22 labels, each of them representing a problem type that may appear during a flight.

#### Yahoo-Arts, Yahoo-Business, Yahoo-Computers, Yahoo-Education, Yahoo-Entertainment, Yahoo-Health, Yahoo-Recreation, Yahoo-Reference, Yahoo-Science, Yahoo-Social, Yahoo-Society

*N. Ueda, K. Saito: Parametric mixture models for multi-labeled text, In Neural Information Processing Systems (NIPS), pp. 737-744, 2002.*

A collection of text classification datasets. The goal is to annotate web pages with top-level and second-level categories.

#### Yeast

*Andre Elisseeff and Jason Weston. A kernel method for multi-labelled classification. In Advances in Neural Information Processing Systems, 14: pp. 681–687, 2001.*

This dataset contains micro-array expressions and phylogenetic profiles for 2,417 yeast genes. Each gene is annoted with a subset of 14 functional categories (e.g., metabolism, energy, etc.) of the top-level of the functional catalogue.