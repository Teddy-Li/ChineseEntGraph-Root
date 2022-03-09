# Chinese Entailment Graph

This repository hosts the links to the collection of programs used in the process of constructing and 
evaluating our Chinese Entailment Graph EG<sub>*Zh*</sub> and its baselines. Behind each link is
a self-containing repository hosting codes serving a certain purpose. These repositories include:

- Open Relation Extraction
    - [ORE_method](): includes our method for extracting open relations from source corpora, as described in 
    section 3.
- Fine-grained Entity Typing
    - [CFIGER](): includes our code for mapping ultra-fine-grained entity types to FIGER type labels; also includes
    the CFET baseline adapted for use in CFIGER ontology. Details described in Section 4.
    - [HierType](): includes code adapted from [Chen et al. 2020](https://github.com/ctongfei/hierarchical-typing).
    The code can now run on the Chinese CFIGER ontology. Details described in Section 4.
- Glue scripts
    - [NE_Pipeline](): the collection of glue programs, putting together results from ORE and FET, returns typed relation
    triples in the input format of entailment graph construction. This repository is central to our project.
- EntGraph Construction
    - [entGraph_Zh](): the program adapted from [Hosseini et al. 2018](https://github.com/mjhosseini/entGraph),
    which is now ready to build Chinese entailment graphs from various source corpora with various ORE methods and entity 
    typing strategies.
- Evaluation
    - [LevyHolt_Chinese](): includes code for the translate-then-parse process for converting the 
    Levy-Holt predicate entailment detection dataset into Chinese. Details described in Section 6.
    - [entgraph_eval_chinese](): includes code for evaluating Chinese entailment graphs and their
    baselines on the predicate entailment detection task. Details described in Section 6 and Section 7.

Each of the above repositories have their own README files, in which the details on how to use them are contained.
