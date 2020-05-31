# Generalized-Semantic-Filter-for-Glossary

This repository contains the automatically extracted glossary terms considering two important qualitative attributes, i.e. feature and benefit of the original CrowdRE requirement specifications dataset. In the original CrowdRE dataset, each entry has 6 attributes, i.e., role, feature, benefit, domain, tags and date-time of creation. Since, we are interested in extracting domain-specific terms from this dataset, we only focus on feature and benefit attributes of this dataset. The dataset used in our experiments containing only the feature and benefit attributes of the original CrowdRE dataset can be viewed in the file named "CrowdRE Requirements Dataset.csv". However, the original CrowdRE dataset is devloped by P. K. Murukannaiah et al. and can be accessed from "The smarthome crowd requirements dataset", https://crowdre.github.io/murukannaiah-smarthome-requirements-dataset/, April, 2017.

For computing the glossary set, we have used the same ground truth set as used in our previous work ("Siba Mishra, Arpit Sharma. Automatic Word Embeddings-Based Glossary Term Extraction from Large-Sized Software Requirements, REFSQ 2020, pp. 203-218.'') which is computed from a random subset of 100 requirement specifications of the used CrowdRE dataset. The ground truth terms have been calculated from our intuition and also utilizing some existing ground truth set ("T. Gemkow, M. Conzelmann, K. Hartig and A. Vogelsang, Automatic Glossary Term Extraction from Large-Scale Requirements Specifications, IEEE 26th International Requirements Engineering Conference (RE), 2018, pp. 412-417.") in an unbiased manner, as there exists no benchmark or gold standard related to the ground truth, whereas the glossary terms are extracted and included in the final set based on the computed semantic similarity scores using the word embedding based fasttext model. The file "Glossary Terms.csv" highlights the extracted glossary terms (a total of 297).

Further, the binary file based on the trained word embedding based fastext model is shared in "generic_filterft200w5.bin". The interested readers are encouraged to cross-check the binary file. For all the glossary terms, the semantic similarity scores are computed using the above mentioned binary file, which have been trained using fastext. 
