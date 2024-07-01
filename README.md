![LLMs4OL: Large Language Models for Ontology Learning](llms4ol-header.jpg)

<H2 style="color: #000080; text-align: center;"><p align="center"> LLMs4OL: Large Language Models for Ontology Learning  </p></H2>
<H3 style="text-align: center;"><p align="center">LLMs4OL Challenge @ ISWC 2024  </p> </H3>
<H3 style="text-align: center;"><p align="center"><a href="https://sites.google.com/view/llms4ol">Website</a> | 
<a href="https://codalab.lisn.upsaclay.fr/competitions/19547 ">Codalab</a></p> </H3>

## Tasks
The LLMs4OL Challenge consists of 3 tasks:

* **Task A - Term Typing**: Discover the generalized type for a lexical term.
* **Task B - Taxonomy Discovery**: Discover the taxonomic hierarchy between type pairs.
* **Task C - Non-Taxonomic Relation Extraction**: Identify non-taxonomic, semantic relations between types.

## Evaluation Phases
Two main evaluation phases for the challenge are:

### 1. Few-shot testing phase
Each ontology selected for system training will be divided into two parts: one part will be released for the training of the systems and another part will be reserved for the testing of systems in this phase. Furthermore, the evaluations will be conducted in two stages of consecutive time windows. In the first stage, only the test datasets for Task A will be released. Then the first stage evaluation window will be declared closed, i.e. no more submissions post the stage 1 evaluation period will be evaluated. Upon closing stage 1, the evaluations for stage 2 will commence. In stage 2, the test dataset for Tasks B and C will be released. This is deliberately planned to disallow for any new term types released in Task B or C test sets to influence systems' performance on the Task A test set.


### 2. Zero-shot testing phase
The zero-shot testing phase will also be organized into two stages that will run in parallel with the few-shot testing phase. The only difference is that new ontologies unseen during training will be introduced. The first stage will test for Task A and the subsequent stage will test for Tasks B and C. The zero-shot testing phase objective is to evaluate the generalizability and transferability of the LLMs developed in this challenge.   

## Datasets

|                    Task                    |   Task No    |        Ontology         |   Train set status   |             Test set status             |
|:------------------------------------------:|:------------:|:-----------------------:|:--------------------:|:---------------------------------------:|
|            Task A - Term Typing            |   A.1 (FS)   |         WordNet         |      `released`      |               `released`                |
|            Task A - Term Typing            |   A.2 (FS)   |        GeoNames         |      `released`      |               `released`                |
|            Task A - Term Typing            |   A.3 (FS)   |      UMLS (SNOMED)      | `released privately` |          `released privately`           |
|            Task A - Term Typing            |   A.3 (FS)   |       UMLS (NCI)        | `released privately` |          `released privately`           |
|            Task A - Term Typing            |   A.3 (FS)   |      UMLS (MEDCIN)      | `released privately` |          `released privately`           |
|            Task A - Term Typing            |   A.4 (FS)   | GO (Biological Process) |      `released`      |               `released`                |
|            Task A - Term Typing            |   A.4 (FS)   | GO (Cellular Component) |      `released`      |               `released`                |
|            Task A - Term Typing            |   A.4 (FS)   | GO (Molecular Function) |      `released`      |               `released`                |
|            Task A - Term Typing            | **A.5 (ZS)** |         Unknown         |          -           |               `released`                |
|            Task A - Term Typing            | **A.6 (ZS)** |         Unknown         |          -           |               `released`                |
|        Task B - Taxonomy Discovery         |   B.1 (FS)   |        GeoNames         |      `released`      |       `releases on July 5, 2024`        |
|        Task B - Taxonomy Discovery         |   B.2 (FS)   |       Schema.org        |      `released`      |       `releases on July 5, 2024`        |
|        Task B - Taxonomy Discovery         |   B.3 (FS)   |          UMLS           | `released privately` |    `privately releases July 5, 2024`    |
|        Task B - Taxonomy Discovery         |   B.4 (FS)   |           GO            |      `released`      |       `releases on July 5, 2024`        |
|        Task B - Taxonomy Discovery         | **B.5 (ZS)** |         Unknown         |          -           |       `releases on July 5, 2024`        |
|        Task B - Taxonomy Discovery         | **B.6 (ZS)** |         Unknown         |          -           |       `releases on July 5, 2024`        |
| Task C - Non-Taxonomic Relation Extraction |   C.1 (FS)   |          UMLS           | `released privately` |    `privately releases July 5, 2024`    |
| Task C - Non-Taxonomic Relation Extraction |   C.2 (FS)   |           GO            |      `released`      |       `releases on July 5, 2024`        |
| Task C - Non-Taxonomic Relation Extraction | **C.3 (ZS)** |         Unknown         |          -           |       `releases on July 5, 2024`        |
| Task C - Non-Taxonomic Relation Extraction | **C.4 (ZS)** |         Unknown         |          -           |       `releases on July 5, 2024`        |

* `FS` stands for Few-shot testing tasks
* `ZS` stands for Zero-shot testing tasks

