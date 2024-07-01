![LLMs4OL: Large Language Models for Ontology Learning](llms4ol-header.jpg)

<H1 style="color: #000080; text-align: center;"><strong>LLMs4OL: Large Language Models for Ontology Learning</strong></H1>
<H3 style="text-align: center;">LLMs4OL Challenge @ ISWC 2024</H3>
<H5 style="text-align: center;"><a href="https://sites.google.com/view/llms4ol">Website</a> | 
<a href="https://codalab.lisn.upsaclay.fr/competitions/19547 ">Codalab</a> </H5>

---

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

|                    Task                    |   Task No    |        Ontology         |
|:------------------------------------------:|:------------:|:-----------------------:|
|            Task A - Term Typing            |   A.1 (FS)   |         WordNet         |
|            Task A - Term Typing            |   A.2 (FS)   |        GeoNames         |
|            Task A - Term Typing            |   A.3 (FS)   |      UMLS (SNOMED)      |
|            Task A - Term Typing            |   A.3 (FS)   |       UMLS (NCI)        |
|            Task A - Term Typing            |   A.3 (FS)   |      UMLS (MEDCIN)      |
|            Task A - Term Typing            |   A.4 (FS)   | GO (Biological Process) |
|            Task A - Term Typing            |   A.4 (FS)   | GO (Cellular Component) |
|            Task A - Term Typing            |   A.4 (FS)   | GO (Molecular Function) |
|            Task A - Term Typing            | **A.5 (ZS)** |         Unknown         |
|            Task A - Term Typing            | **A.6 (ZS)** |         Unknown         |
|        Task B - Taxonomy Discovery         |   B.1 (FS)   |        GeoNames         |
|        Task B - Taxonomy Discovery         |   B.2 (FS)   |       Schema.org        |
|        Task B - Taxonomy Discovery         |   B.3 (FS)   |          UMLS           |
|        Task B - Taxonomy Discovery         |   B.4 (FS)   |           GO            |
|        Task B - Taxonomy Discovery         | **B.5 (ZS)** |         Unknown         |
|        Task B - Taxonomy Discovery         | **B.6 (ZS)** |         Unknown         |
| Task C - Non-Taxonomic Relation Extraction |   C.1 (FS)   |          UMLS           |
| Task C - Non-Taxonomic Relation Extraction |   C.2 (FS)   |           GO            |
| Task C - Non-Taxonomic Relation Extraction | **C.3 (ZS)** |         Unknown         |
| Task C - Non-Taxonomic Relation Extraction | **C.4 (ZS)** |         Unknown         |

* `FS` stands for Few-shot testing tasks
* `ZS` stands for Zero-shot testing tasks

