# Replication Package for "The Impact of Classifier Configuration and Combination on Bug Localization"

Stephen W. Thomas, Meiyappan Nagappan, Dorothea Blostein, and Ahmed E. Hassan  
[IEEE Transactions on Software Engineering, vol. 39, issue 10, 2013](http://dx.doi.org/10.1109/TSE.2013.27)

Abstract: Bug localization is the task of determining the source code entities that are relevant to a new bug report. Manual bug localization is labor intensive, since a developer must consider hundreds or thousands of source code entities. Current research builds bug localization classifiers, based on information retrieval models, to locate entities that are textually similar to a given bug report. Current research, however, does not consider the effect of classifier configuration, i.e., all the parameter values that specify the exact behavior of the classifier. As such, it is unknown how important each parameter is, or which particular parameter values lead to the best overall bug localization performance. In this paper, we empirically investigate the effectiveness of a large space of classifier configurations, 3,172 in total. Further, we introduce a framework for combining the results of multiple classifier configurations, a technique which has shown promise in many other domains. Through a detailed case study on over 8,000 bug reports from three real-world systems, we determine (a) that the parameters of a classifier have a significant impact on its performance, and therefore practitioners and researchers must consider them carefully, and (b) that combining multiple classifiers improves the performance of even the best individual classifiers, often by significant amounts. Our results substantially improve the state-of-the-art in bug localization.

## BibTeX

```bibtex
@ARTICLE{ThomasTSE13,
author={S. W. Thomas and M. Nagappan and D. Blostein and A. E. Hassan},
journal={IEEE Transactions on Software Engineering},
title={The Impact of Classifier Configuration and Classifier Combination on Bug Localization},
year={2013},
volume={39},
number={10},
pages={1427-1443},
doi={10.1109/TSE.2013.27},
ISSN={0098-5589},
month={Oct}
}
```

## Data and Scripts

- Ground Truth Data:
  - [Bug-code links](https://github.com/SAILResearch/replication-classifier_conf_config_bugloc/files/1738073/bugs-to-files.zip)
- Case Study 1: Component Classifier Investigation
  - [All classifier results (all systems, all metrics, IR- and EM-based classifiers)](https://github.com/SAILResearch/replication-classifier_conf_config_bugloc/files/1490023/all-classifier-results.zip)
  - [HSD results (all systems, all factor levels, top-20 metric)](https://github.com/SAILResearch/replication-classifier_conf_config_bugloc/files/1490036/hsd-results.zip)
  
- Case Study 2: Classifier Combination
  - [All results (all systems, all metrics, all classifier combinations)](https://github.com/SAILResearch/replication-classifier_conf_config_bugloc/files/1490023/all-classifier-results.zip)
  - [View randomly-selected classifiers (CSV format)](https://github.com/SAILResearch/replication-classifier_conf_config_bugloc/files/1490026/randomly-selected-classifiers.zip)
  
An interactive visualization of the results can be found [here](http://sailhome.cs.queensu.ca/replication/sthomas/TSE2013/bl/results.html).

## Tools

Our ```lscp``` preprocessing tool is also on [GitHub](https://github.com/stepthom/lscp).

Our ```lucene-lda``` LDA-based BL tool is also on [GitHub](https://github.com/stepthom/lucene-lda). 
