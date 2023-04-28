# MTL3_EventDetection

This repository contains the codebase of the paper EDM3: Event Detection as Multi-task Text Generation.

The scripts required for data preprocessing and preparation from their native form, as well as post-processing and evaluation can be found here.

## EDM3: An Overview 

Event detection refers to identifying event occurrences in a text and comprises two subtasks; event identification and classification.

In this work, we reformulate Event Detection as three generative tasks: identification, classification, and combined detection and propose Event Detection as Multi-task Text Generation: EDM3. 

We evaluate EDM3 on multiple event detection datasets, showing that EDM3 outperforms 1) single-task performance by 8.4\% on average and 2) multi-task performance without instructional prompts by 2.4% on average.
We obtain SOTA results on RAMS (71.3% vs. 65.1% F-1) and competitive performance on other ED datasets.

We break ED down into its atomic subtasks, and then reformulate these simpler tasks, along with the complex primary task, generatively.
<p align="center">
<img width="606" alt="image" src="https://user-images.githubusercontent.com/28482281/235067068-b1beaed7-11d7-4e71-bd47-7f1626bbe996.png">
</p>

We show that by modeling ED and its subtasks as individual, similarly-formatted sequence generation tasks, a model can learn transferable knowledge from the subtasks that can be leveraged to improve performance on ED. 
Additionally, by leveraging instruction tuning, we utilize the wealth of pretrained knowledge available to generative language models, allowing EDM3 to be utilized over any classification schema.

<p align="center">
<img width="568" alt="image" src="https://user-images.githubusercontent.com/28482281/235067240-4b018dd4-48db-4ae0-8834-2412dc9af48f.png">
</p>



