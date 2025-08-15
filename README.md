**Important:** Due to file sizes, lora_adapters can be reached through here: https://drive.google.com/drive/folders/1M_zupYKwMso5r5ibYMzNiTxg--89sf-0?usp=drive_link

# A Hybrid Post-Hoc Feedback Framework for Latin Dactylic Hexameter

This repository contains the code and resources for the master's thesis, "A Hybrid Post Hoc Feedback Framework for Latin Dactylic Hexameter: Experiments with Transformer Models on Contemporary Themes."

**Abstract**
This research investigates the challenge of generating metrically correct Latin dactylic hexameter on contemporary themes using modern transformer models. The core of this research is a hybrid system that combines the creative potential of fine-tuned Large Language Models (LLMs) with the formal rigor of a symbolic, rule-based validator.

A series of experiments were conducted across several models from the Llama and Gemma families. These models were fine-tuned on four custom datasets, each designed for a specific purpose: V1/V2 established a baseline with core classical authors and tested the use of special tokens; V3 expanded the corpus with more authors to improve generalization; and V4 introduced synthetically generated poems on modern topics to adapt an instruction-tuned model for contemporary themes. The generation process uses an iterative feedback loop: the LLM generates a line of poetry, which is then validated for metrical correctness by the Classical Language Toolkit (CLTK). If a line fails validation, it is discarded and regenerated.

The findings indicate that larger, instruction-tuned models like Gemma 3 12B-IT produce the most semantically coherent and stylistically convincing verse. While many models were tested, the final generation code in 3_Poetry_Generator.ipynb is specifically configured for the two most successful models: gemma-3-12b-pt (for classical generation) and gemma-3-12b-it (for contemporary generation). However, achieving consistent metrical accuracy proved challenging, primarily due to limitations in the CLTK's validation tools. This research involves a framework for computational creativity in historical languages and provides a detailed analysis of the current capabilities and limitations of LLMs in handling complex poetic forms.
