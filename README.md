# mte-zh-mwe
<!-- Copyright [19 Mar 2024] [florethsong]  

 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at

    http://www.apache.org/licenses/LICENSE-2.0

 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.-->
---
The extended dataset of the WMT22 Metrics Shared Task with the identification of translation errors (based on multidimensional quality metrics) directly related to Chinese Multiword Expressions (MWEs). The annotations of MWEs are provided by: https://github.com/florethsong/mtme-zh-mwe.
---

### :card_index_dividers: Description of file structure
```
.
│  all.json # Annotation results of all Chinese MWEs in the WMT22 zh-en source text provided by Song and Xu (2024)
│  cat.json  # List of all annotated Chinese MWE items grouped by categories (non-deduplicated) provided by Song and Xu (2024)
│  translation_errors_with_mwe_annotation.tsv # MQM-based translation error annotations by WMT22 (Freitag et al., 2022), extended with Chinese MWE labels showing what kinds of MWEs the errors are directly related to.
│  
└─raw_wmt22 # Original dataset from WMT22 Metric Sharted Task (Freitag et al., 2022), including source texts, machine translation system outputs, references, and human evaluation scores, 
    ├─human-scores
    │      zh-en.mqm.seg.score
    │      zh-en.wmt-appraise-z.seg.score
    │      zh-en.wmt-appraise.seg.score
    │      zh-en.wmt-z.seg.score
    │      zh-en.wmt.seg.score
    │      
    ├─references
    │      zh-en.refA.txt
    │      zh-en.refB.txt
    │      
    ├─sources
    │      zh-en.txt
    │      
    └─system-outputs
        └─zh-en
                AISP-SJTU.txt
                bleurt_bestmbr.txt
                bleu_bestmbr.txt
                chrf_bestmbr.txt
                comet_bestmbr.txt
                DLUT.txt
                HuaweiTSC.txt
                JDExploreAcademy.txt
                Lan-Bridge.txt
                LanguageX.txt
                M2M100_1.2B-B4.txt
                NiuTrans.txt
                Online-A.txt
                Online-B.txt
                Online-G.txt
                Online-W.txt
                Online-Y.txt
                QUARTZ_TuneReranking.txt
                refA.txt
                refB.txt
```
## Citation
Please cite the following paper if it is helpful to your work :)!



## References
Markus Freitag, Ricardo Rei, Nitika Mathur, Chikiu Lo, Craig Stewart, Eleftherios Avramidis, Tom Kocmi, George Foster, Alon Lavie, and André F. T. Martins. 2022. [Results of WMT22 metrics shared task: Stop using BLEU - neural metrics are better and more robust](https://aclanthology.org/2022.wmt-1.2). In Proceedings of the Seventh Conference on Machine Translation (WMT), pages 46–68, Abu Dhabi, United Arab Emirates (Hybrid). Association for Computational Linguistics.  

Huacheng Song and Hongzhi Xu. 2024. [Benchmarking the performance of machine translation evaluation metrics with Chinese multiword expressions](https://aclanthology.org/2024.lrec-main.198). In Proceedings of the 2024 Joint International Conference on Computational Linguistics, Language Resources and Evaluation (LREC-COLING 2024), pages 2204–2216, Torino, Italia. ELRA and ICCL.
