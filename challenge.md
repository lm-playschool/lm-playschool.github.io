---
layout: page
title: Challenge
playschool_title: true
show_mailing_list: true
---

## A Playschool for LLMs

Despite the great advancements accomplished by the community in both training and post-training methodologies, at the moment models are still lacking a wide range of key collaborative interactional competences that human language users possess, even when provided with much larger amounts of data.

With the goal of overcoming such limitations of current training regimes, the **LM Playschool Challenge** targets significant advances in the efficient development of collaborative AI systems and promotes research on training regimes that are best suited for creating agentic conversational language models (ACLMs).

The **LM Playschool Challenge** therefore poses the following questions:
* How can we efficiently improve pre-trained LMs towards modelling a collaborative language understander and user?
  * More specifically, what role can structured interaction with another agent play in the training process?

Why a **Playschool**?<br>
The focus of the competition are pre-trained (and instruction-tuned) models which, metaphorically are still children when compared to humans but are not newborn babies anymore. Similarly to them, they are therefore ready to join a place (the [**Playschool**](https://www.collinsdictionary.com/dictionary/english/playschool)), where they can engage in structured, interactive activities with others and potentially strengthening their collaborative and general language use capabilities.

<br>

## About the Challenge

The LM Playschool Challenge investigates how pre-trained language models can be efficiently post-trained to acquire collaborative interactional competences through structured dialogue. Participating teams will develop training regimes that improve a model's ability to generalise to unseen goal-oriented dialogue games, while preserving performance on standard NLP benchmarks and cognitive tests.

**Central research question:** How can we best improve a pre-trained LM's capacity as a collaborative language user — and what role does structured agent interaction play in that process?

<br>

## Provided Resources (Starter Pack)

A starter pack will be released in **late March 2026** containing everything needed to begin development:

| Resource | Description |
|----------|-------------|
| Training data | Existing dialogue transcripts (suitable for SFT-style training) and game instances (suitable for online RL and related approaches) |
| Evaluation data | Held-out game instances not included in the training set, plus standard static benchmarks |
| Base models | A tentative list of latest models will be provided |
| Sample code | Jupyter notebooks with reference training and evaluation scripts |

<br>

## Submission Requirements

### 1. System Submission

Each team submits a trained model for evaluation. The following are required:

**Model artefact**: Provide a publicly accessible **Hugging Face model URL** containing the post-trained model with **full merged weights**.

**Inference compatibility**: If the submitted model is not supported by the provided libraries, teams must additionally provide:
- **Dockerized setup** that allows to run the trained model, e.g. expose an **OpenAI-Compatible API** endpoint

**Documentation**: Submit a **model training card** that covers: training methodology, data usage breakdown, hyperparameters, compute budget, and any design decisions relevant to reproducibility.
