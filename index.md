# A Playschool for LLMs

> *Playschool: an informal type of school for very young children where they learn things by playing. [Collins](https://www.collinsdictionary.com/dictionary/english/playschool)*

The **LM Playschool Challenge** aims at fostering research on training regimes that are best suited for creating agentic conversational language models (ACLMs). It therefore targets significant advances in the efficient development of collaborative AI systems.

The challenge builds on the observation that current training is partially ineffective, in that the resulting models lack key collaborative interactional competences that human language users have.

The **LM Playschool Challenge** therefore poses the following questions: How can we efficiently improve pre-trained LMs towards modelling a collaborative language understander and user, given a fixed token post-training budget? Specifically, it asks: “What role can structured interaction with a teacher model play in the training process?” 
## What we Provide

The challenge organisers provide a setup (the Playpen) for conducting such structured interactions --- language games, or "Sprachspiel", in Wittgenstein's terminology---, which offers as learning signal both linguistic feedback from a teacher (clarification requests, corrections) as well as feedback from the (interaction) environment (task success or failure), and which provides some control over the training process to the learner. (This will be based on the [clembench](https://github.com/clp-research/clembench) environment, with some modifications that will be released soon.)  

The organisers also provide an evaluation pipeline that operationalises the notion of a "collaborative language understander and user (CLU2)" by mixing established reference-based language understanding evaluation datasets (e.g., MMLU) with novel interactional tests, ensuring that both "internal" skills such as reasoning, understanding, as well as "external" skills such as conversational collaboration and multi-turn coherence establishment are tested.

## Your Task

All participants in the challenge start with the same base model, which will be the best performing (at the time of the start of the challenge) model in the ~10B parameters class, pre-trained to be able to follow instructions. (This motivates the name of the challenge: the **LM Playschool Challenge** is about improving a pre-trained model with a certain budget.)

Participants are free to use whatever method or data they see fit to achieve improvements. Evaluation will be on the CLU2 pipeline mentioned above, with a special prize reserved for the highest improvement on the "collaborative language use" dimension.

Use of the Playpen is encouraged, but not required. Entries to the competition can be (but do not have to be) pure fine-tunes of the base model; agentive systems that wrap the model in additional code (e.g., for introspection or self-regulation) are also welcome.
