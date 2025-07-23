# Reasoning Circuits in Language Models: A Mechanistic Interpretation of Syllogistic Inference

**Authors:**  
Geonhee Kim, Marco Valentino, André Freitas

---

<img src="images/introduction.png" alt="Introduction" style="width:60%;"/>

## Overview

This repository contains the official codebase for the paper:

> **Reasoning Circuits in Language Models: A Mechanistic Interpretation of Syllogistic Inference**  
> Geonhee Kim, Marco Valentino, André Freitas  
> [Findings of ACL 2025](https://aclanthology.org/2025.findings-acl.525/)

The project provides a mechanistic analysis of how large language models perform syllogistic inference, offering insights into the internal reasoning circuits that underpin logical reasoning capabilities in auto-regressive models.

## Project Setup

To install the required dependencies and set up the environment, please run:

```bash
conda create -n mechsyllogism python=3.9 -y
conda activate mechsyllogism

git clone https://github.com/neuro-symbolic-ai/Mechanistic-Interpretation-Syllogism.git
cd Mechanistic-Interpretation-Syllogism/scripts
bash ./install_dependencies.sh
```

After the installation is complete, you can run the demo file `main.ipynb`.

## Citation

If you use this codebase or find our work helpful, please cite:



```bibtex
@inproceedings{kim-etal-2025-reasoning,
    title = "Reasoning Circuits in Language Models: A Mechanistic Interpretation of Syllogistic Inference",
    author = "Kim, Geonhee  and
      Valentino, Marco  and
      Freitas, Andre",
    editor = "Che, Wanxiang  and
      Nabende, Joyce  and
      Shutova, Ekaterina  and
      Pilehvar, Mohammad Taher",
    booktitle = "Findings of the Association for Computational Linguistics: ACL 2025",
    month = jul,
    year = "2025",
    address = "Vienna, Austria",
    publisher = "Association for Computational Linguistics",
    url = "https://aclanthology.org/2025.findings-acl.525/",
    pages = "10074--10095",
    ISBN = "979-8-89176-256-5",
    abstract = "Recent studies on reasoning in language models (LMs) have sparked a debate on whether they can learn systematic inferential principles or merely exploit superficial patterns in the training data. To understand and uncover the mechanisms adopted for formal reasoning in LMs, this paper presents a mechanistic interpretation of syllogistic inference. Specifically, we present a methodology for circuit discovery aimed at interpreting content-independent and formal reasoning mechanisms. Through two distinct intervention methods, we uncover a sufficient and necessary circuit involving middle-term suppression that elucidates how LMs transfer information to derive valid conclusions from premises. Furthermore, we investigate how belief biases manifest in syllogistic inference, finding evidence of partial contamination from additional attention heads responsible for encoding commonsense and contextualized knowledge. Finally, we explore the generalization of the discovered mechanisms across various syllogistic schemes, model sizes and architectures. The identified circuit is sufficient and necessary for syllogistic schemes on which the models achieve high accuracy ($\geq$ 60{\%}), with compatible activation patterns across models of different families. Overall, our findings suggest that LMs learn transferable content-independent reasoning mechanisms, but that, at the same time, such mechanisms do not involve generalizable and abstract logical primitives, being susceptible to contamination by the same world knowledge acquired during pre-training."
}
```