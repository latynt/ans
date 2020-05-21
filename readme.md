ANS: Arabic News Stance Corpus
=========================
![version](https://img.shields.io/badge/version-v0.1-blue) [![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)

An News Titles Stance Dataset in Arabic.  The dataset includes two perspectives as described below.  For details on how the data was created and examples of use, please refer to the paper:

```
Khouja, Jude. “Stance Prediction and Claim Verification: An Arabic Perspective.” 
Proceedings of the Third Workshop on Fact Extraction and VERification workshop at ACL 2020 (FEVER), (2020).
```

### Citation:
If you use this data, please cite the following work:

```
@inproceedings{,
    title = "Stance Prediction and Claim Verification: An {A}rabic Perspective", 
    author = "Khouja, Jude",
    booktitle = "Proceedings of the Third Workshop on Fact Extraction and {VER}ification ({FEVER})",
    month = may,
    year = "2020",
    address = "Seattle, USA",
    publisher = "Association for Computational Linguistics",
}

```

### Examples:

The claim verification version of the data is a binay classification task.  Data contains two columns: claim and fake_flag:

| claim | fake_flag |
|---|---|
|أدنوك تستثمر 165 مليار درهم في التكرير والبتروكيماويات|0|
|أسبوع الموضة العربي في السعودية للمرة العاشرة|1|


The stance prediction version is a 3-class classification task. Data contains three columns: s1, s2, stance:

| s1 | s2 | stance|
|---|---|---|
|مفتشو الأسلحة الكيمياوية يباشرون دورهم في دوما السورية|تأجيل مهمة مفتشي الأسلحة الكيمياوية في دوما السورية|disagree|
|تراجع التضخم في مصر|اعترافات سليمان الحلبي تكشف أسرار مقتل كليبر في مصر|other|

### Usage:
For reproduciblity, we are sharing the dev and test splits. By submitting results using the same splits, you acknowledge that your results are obtained purely by training on the training split and tuned on the dev split (you only evaluted on the test set once).

### Changelog
- v0.1 Initial release
