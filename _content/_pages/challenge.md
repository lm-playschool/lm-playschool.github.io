---
layout: page
title: Challenge
playschool_title: true
show_mailing_list: true
---

## What is this all about?

LLMs are increasingly used as agents that engage in multi-step interactions, yet they are trained either on purely observational data (text corpora) or on single stimulus-response pairs (instructions and replies). Could learning in multi-step conversational interaction (in what we call "dialogue games") improve their agentic capabilities? The LM-Playschool-Challenge aims at finding out.

<details>
<summary>Dialogue games?</summary>
To get a sense of what kind of conversational games we're talking about, you can explore the [clembench transcript browser](https://clembench.github.io/transcript-browser.html). There you can select a game, a model that has played it, an experiment (a set of problems within the game), and finally an instance (an actual problem). This will display the transcript of the two interleaved interactions — between player A and the Game Master (the facilitator of the game), and between the Game Master and player B — that make up an episode of a conversational game. Click around to explore other games and other models. For example, you can switch between models for the same instance to see how they may differ in their game playing abilities. For your experiments, you may either use these transcripts directly, work with the underlying framework used to generate them, or develop your own setup to produce similar synthetic interactions.
</details>


## How does this work?

For this first edition of the challenge, we impose very few constraints on participants. You are free to choose any base model you want as starting point, and you can do whatever you want to it — the point where we all come together is in how the final model will be evaluated. All submissions will be evaluated on an unseen test set of dialogue games drawn from a private version of the clembench framework, and improvement is measured relative to the base model.

We do, however, provide a set of recommendations. We anticipate (and encourage) most participants to work with one of Qwen3.5-0.8B, -2B, -4B, -9B, or -27B — a broad range of model sizes which ensures that you can contribute even with modest computational resources. In addition, since this is the declared main interest of the shared task and the workshop, we strongly encourage the use of interaction data to improve models. To suppor this, we provide participants with the playpen environment, which is related but not identical to the final testing environment, and which includes example games, example learning scripts, and a development evaluation setup. (See below.)

*Table with playpen eval scores of a selection of potential base models (such as the Qwens, but also good old Llama3.1-8B) to be added here.*

## How do I take part?

**Step 1: Come up with a name for your team.** Very important. This will identify your team on the intermediate and final scoreboards, so be creative! (The Powerful Piagets? LanguageSuperModelsRock? All-play-and-no-work? The Bielefeld Beagles? Knock yourself out.)

**Step 2: Register your interest.** Use [this form](https://forms.gle/cDx9wNUU57KJoTiy8) to register your interest in the shared task. This doesn't commit you to anything, but will allow us to gauge interest, and it will allow you to submit intermediate updates (see below). (Please register by April 30th.)

**Step 3: Install the eval pipeline.** Contributions will be evaluated in a common framework. To make sure that this works seamlessly, we ask participants that they perform intermediate evaluations themselves, using a public version of the evaluation framework. This is available at <https://github.com/lm-playpen/playpen>. Follow the instructions under "Set up the playpen workspace" and "Evaluate a model", and make sure that you can perform the evaluation with your model.

**Step 4: Innovate!** Now do something that makes the numbers go up. For inspiration, have a look at the examples on <https://github.com/lm-playpen/playpen>. Feel free to build on these, and on the clembench dialogue games, or come up with your own framework for synthesising interaction data and interactions. If you think it falls under "learning in interaction", it fits.

**Step 5: Check in.** From May 1st on, you can use *this form* (tba) to submit your current best results (as calculated by the eval pipeline). We will update a shared list, so you can see where you stand (relative to others who work with the same base model, or in terms of improvement over the base model that you have achieved). 

**Step 6: Submit your best attempt.** From June 22nd on (and until July 5th), you can use *this form* (tba) to submit the model (or models) that you want to be considered for the final evaluation. For this, you will submit a link to a model uploaded to huggingface. Also provide a model training card that covers: training methodology, data usage breakdown, hyperparameters, compute budget, and any design decisions relevant to reproducibility.

We will take this model and run it on the private evaluation pipeline, which is similar, but not identical to the one you had access to during the development phase.

**Step 7: Write up what you did.** Write up all the great things you've learned during step 4, and submit to the workshop! (Also include the model training card here, and expand on the information provided therein.)

**Step 8: Enjoy the workshop.** Come to Budapest on 24-29 October (exact EMNLP workshop dates TBD), and enjoy the presentations (and hopefully give one yourself). A selection committee will have selected three *best papers*, according to criteria such as *scientific impact of explored method*, *insight*, *innovation*, etc. Maybe your paper will be one of these?



## What's in it for me?

Fame and fortune! Or (as there are no cash prizes to be won, unfortunately) at least fame! Insofar as getting a spot at an EMNLP workshop gives you that. 


## How can I reach you?

Use the issue tracker at <https://github.com/lm-playpen/playpen/issues> to post questions about the shared task specifically (like problems evaluating your model, questions about what exactly to submit, etc.) and issues with the playpen example code specifically. (Please make sure that you have a look at the closed issues before posting a new one; maybe your problem has already been addressed.)


## What can I do?

Here's an unsorted, unstructured and unverified list of ideas to try out:
- Incorporate intrinsic reward signals (e.g., curiosity, uncertainty reduction, task progress)
- Fine-tune on trajectories filtered by success or high-quality interaction patterns
- Learn a reward model from game transcripts and optimise against it
- Distil stronger "teacher" models into smaller "student" (e.g., using a "caregiver" agent that provides corrective feedback during training)
- Train models to explicitly track and update beliefs about the game state
- Try out multi-turn RL approaches
- Use planning-augmented decision making mechanisms (i.e., simulate future dialogue turns and environment states before acting)
