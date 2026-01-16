---
layout: challenge
---

# A Playschool for LLMs

Despite the great advancements accomplished by the community in both training and post-training methodologies, at the moment models are still lacking a wide range of key collaborative interactional competences that human language users possess, even when provided with much larger amounts of data.

With the goal of overcoming such limitations of current training regimes, the **LM Playschool Challenge** targets significant advances in the efficient development of collaborative AI systems and promotes research on training regimes that are best suited for creating agentic conversational language models (ACLMs).


The **LM Playschool Challenge** therefore poses the following questions:
* How can we efficiently improve pre-trained LMs towards modelling a collaborative language understander and user, given a fixed token post-training budget? 
  * More specifically, what role can structured interaction with another agent play in the training process? 

Why a **Playschool**?  
The focus of the competition are pre-trained (and instruction-tuned) models which, metaphorically are still children when compared to humans but are not newborn babies anymore. Similarly to them, they are therefore ready to join a place (the [**Playschool**](https://www.collinsdictionary.com/dictionary/english/playschool)), where they can engage in structured, interactive activities with others and potentially strengthening their collaborative and general language use capabilities.

## What we Provide

The challenge organisers provide a setup (the Playpen) for conducting such structured interactions --- language games, or "Sprachspiel", in Wittgenstein's terminology---, which offers as learning signal both linguistic feedback from a teacher (clarification requests, corrections) as well as feedback from the (interaction) environment (task success or failure), and which provides some control over the training process to the learner. (This will be based on the [clembench](https://github.com/clp-research/clembench) environment, with some modifications that will be released soon.)

{%- include taboo-sample.html -%}

The organisers also provide an evaluation pipeline that operationalises the notion of a "collaborative language understander and user (CLU2)" by mixing established reference-based language understanding evaluation datasets - many of which inspired by cognitive science literature - (e.g., BBH, MMLU-Pro) with novel interactional tests, ensuring that both "internal" skills such as reasoning, understanding, as well as "external" skills such as conversational collaboration and multi-turn coherence establishment are tested.

## Your Task

All participants start with the same base model, selected within the 8B parameters class, pre-trained to be able to follow instructions.

There are no limitations regarding the type of data that is allowed for training models, with the only limitations being put on the amount of data that can be used. This means, not making use of interactive approaches at all is perfectly fine. This competition is a unique opportunity to compare interactive, non-interactive and hybrid training regimes on both interactive as well as non-interactive benchmarks (the CLU2 pipeline mentioned above) and highlight their respective strenghts and weaknesses with respect to each other. 

Use of the Playpen is encouraged, but not required. Entries to the competition can be (but do not have to be) pure fine-tunes of the base model; agentive systems that wrap the model in additional code (e.g., for introspection or self-regulation) are also welcome.

Prizes are offered to the best-performing models on the provided evaluation pipeline.

## Contacts

Join the mailing list to get updated regarding the competition, [here](https://www.listserv.dfn.de/sympa/subscribe/llm-playschool-challenge).
