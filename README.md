# KG-FPQ: Evaluating Factuality Hallucination in LLMs with Knowledge Graph-based False Premise Questions
<p align="center">
  <a href="https://arxiv.org/abs/2407.05868">
    <img src="https://img.shields.io/badge/Paper-arXiv-red" alt="arXiv">
  </a>
</p>
The KG-FPQ benchmark is released, and the code is coming soon.

## Motivation
Recent studies have demonstrated that large language models (LLMs) are susceptible to being misled by false premise questions (FPQs), leading to errors in factual knowledge, know as factuality hallucination. Existing benchmarks that assess this vulnerability primarily rely on manual construction, resulting in limited scale and lack of scalability. In this work, we introduce an automated, scalable pipeline to create FPQs based on knowledge graphs (KGs). The first step is modifying true triplets extracted from KGs to create false premises. Subsequently, utilizing the state-of-the-art capabilities of GPTs, we generate semantically rich FPQs. Based on the proposed method, we present a comprehensive benchmark, the Knowledge Graph-based False Premise Questions (KG-FPQ), which contains approximately 178k FPQs across three knowledge domains, at six levels of confusability, and in two task formats. Using KG-FPQ, we conduct extensive evaluations on several representative LLMs and provide valuable insights. 
<p align="center">
  <img src="images/example.png" alt="An example of a FPQ." width="400">
</p>

## Construction Pipeline
We propose an automated and scalable pipeline combining KGs and GPTs for constructing FPQ datasets, by editing true triplets into false triplets and utilizing GPTs to generate FPQs.
<p align="center">
  <img src="images/data constructing.png" alt="Construction Pipeline." width="800">
</p>
<p align="center">
  <img src="images/editing.png" alt="Editing methods." width="800">
</p>

## Citation
@article{zhu2024kgfpqevaluatingfactualityhallucination,
      title={KG-FPQ: Evaluating Factuality Hallucination in LLMs with Knowledge Graph-based False Premise Questions}, 
      author={Yanxu Zhu and Jinlin Xiao and Yuhang Wang and Jitao Sang},
      year={2024},
      eprint={2407.05868},
      archivePrefix={arXiv},
      primaryClass={cs.CL},
}
