# InDepth-Eva-MRC
InDepth-Eva-MRC is an interactive and visualized platform to provide analysis from cognitive fine-grained for Machine Reading Comprehension(MRC) models.

The platform makes post-hoc systems to explain the behavior of MRC models. On the one hand, it analyzes the linguistic bias via performances with different linguistic properties. On the other hand, it performs skill-based analysis methods based on the modified test samples and semi-automatically generated test samples. Furthermore, through its detailed and interactive visualizations, the platform offers in-depth results analysis and model comparison from cognitive fine-grained.

The complete install and quick start documents are coming soon, and the demonstration video is available at [there](https://github.com/py-rgb/InDepth-Eva-MRC/blob/main/InDepth-Eva-MRC-Video.mp4) and [YouTube](https://youtu.be/MB_0exH0x0Q).


## :couple: Audiences
* **Researchers:** InDepth-Eva-MRC can easily help you to view the baseline model of MRC task, and provide fine-grained evaluation analysis of the model.
* **New to MRC:** InDepth-Eva-MRC can quickly help you understand the process of mrc tasks, and can also make you understand the model more clearly through fine-grained analysis.

## Main Supported Functionality 
* Preloads several MRC models and datasets, and provides the user interface to quickly train an MRC model.
* Provides fine-grained evaluation analysis of the pre-loaded model.
* Provides interface to support new users’ model analysis.

We hope that the InDepth-Eva-MRC platform can facilitate the advancement of cognitive evaluation with more human-like reasoning skills.

## Overview Architecture
![alt 属性文本](./src/framework.png )
Our system consists of five main modules: 
* MRC Datasets
   * preloads five extractive MRC datasets: SQuAD 1.1, HotpotQA, Natural Questions, NewsQA, and TriviaQA.
   * manages datasets and provides basic operations, such as add, delete, update and search.
* MRC Models
   * preloads six popular MRC models: BIDAF, R-NET, BERT, Span-BERT, BLANC and GPT2.
   * provides the user interface to quickly train an MRC model by adjusting the corresponding hyper-parameters and training dataset.
* Principles for In-depth Analysis
   * describes three principles for in-depth analysis, including 1) linguistic bias analysis based on the original test sets; 2)internal skill-based analysis based on new reconstructed test sets; and 3) external skill-based analysis based on new generated test sets.
   * provides a flexible interface to reconstruct new test sets for internal skill-based analysis.
   * The complete principles, along with corresponding case examples and analysis strategies, are available at [Analysis Principles Document](https://github.com/py-rgb/InDepth-Eva-MRC/tree/main/Analysis%20Principles%20Document).
* Evaluation
   * evaluates the trained MRC model on the original new test sets and lists all results and supports illustrating each sample for a case study.
   * users can also download all kinds of test sets and upload their prediction files to the platform.
* Analysis & Visualization
   * Visualization for Single Model
      * linguistic bias analysis
      * internal skill-based analysis
      * external skill-based analysis
   * Visualization for Model Comparison
      * provides cognitive comparison between two different MRC models.
      * presents the comparsion, conclusion and case studies for three analysis principles.

   
## How to Use
In conclusion, InDepth-Eva-MRC platform offers thorough cognitive evaluation and fine-grained comparison of MRC models from three analysis principles. Besides, uesrs can also download all kinds of test sets and upload their prediction files to the platform, so as to anslysis their own MRC models.

The screenshots and additional external material are available at [screenshots](https://github.com/py-rgb/InDepth-Eva-MRC/tree/main/screenshots).

## Install & Quick Start
[Code](https://github.com/distantJing/InDepth-Eva-MRC/tree/main/Code)

## References
```
Marco Túlio Ribeiro, Tongshuang Wu, Carlos Guestrin, Sameer Singh: Beyond Accuracy: Behavioral Testing of NLP Models with CheckList. ACL 2020: 4902-4912

Saku Sugawara, Pontus Stenetorp, Kentaro Inui, Akiko Aizawa: Assessing the Benchmarking Capacity of Machine Reading Comprehension Datasets. AAAI 2020: 8918-8927
```
