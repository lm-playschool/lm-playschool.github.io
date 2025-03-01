---
layout: page
title: LM Playschool Challenge
---

![SHARED TASK LOGO](https://drive.google.com/file/d/1umxPpJn8Xdoicx4iPGeuAHV_mB5-AeQ0/view?usp=drive_link)

## The Goal
The PlaySchool-LM challenge  aims at fostering research on training regimes that are best suited for creating agentic conversational language models (ACLMs).  It therefore targets significant advances in the efficient development of collaborative AI systems. We are requesting sponsorship support to develop and run the challenge. 

The challenge builds on the observation that current training is partially ineffective, in that the resulting models lack key collaborative interactional competences that human language users have. 

The  Playschool-LM challenge therefore poses the following questions: How can we efficiently improve pre-trained LMs towards modelling a collaborative language understander and user, given a fixed token post-training  budget?  Specifically, it asks ``What role can structured interaction with a teacher model play in the training process?’’ 

## What we Provide
  The challenge organisers provide a setup (the Playpen) for conducting such structured interactions, which offers as learning signal both linguistic feedback from a teacher (clarification requests, corrections) as well as feedback from the (interaction) environment (task success or failure), and which provides some control over the training process to the learner. The organisers also provide an evaluation pipeline that operationalises the notion of a "collaborative language understander and user (CLU2)"  by mixing established reference-based language understanding evaluation datasets (e.g., MMLU) with novel interactional tests, ensuring that both "internal" skills such as reasoning, understanding, as well as "external" skills such as conversational collaboration and multi-turn coherence establishment are tested.
## Your Task
All participants in the challenge start with the same base model, which will be the best performing (at the time of the start of the challenge) model in the ~10B parameters class, pre-trained to be able to follow instructions. (This motivates the name of the challenge: the PlaySchool-LM challenge is about improving a pre-trained model with a certain budget.)

Participants are free to use whatever method or data they see fit to achieve improvements. Evaluation will be on the CLU2 pipeline mentioned above; with a special prize reserved for the highest improvement on the "collaborative language use" dimension. Use of the Playpen is encouraged, but not required. Entries to the competition can be (but do not have to be) pure fine-tunes of the base model; agentive systems that wrap the model in additional code (e.g., for introspection or self-regulation) are also welcome.

# Organizers
* Raffaella Bernardi (Uni Trento)
* Raquel Fernández (Uni Amsterdam)
* Mario Giulianelli (ETH Zurich)
* Alexander Koller (Saarland Uni)
* Oliver Lemon (Heriot-Watt Uni)
* David Schlangen (Uni Potsdam)
* Alessandro Suglia (Heriot-Watt Uni)
* ALL THE OTHER NAMES
