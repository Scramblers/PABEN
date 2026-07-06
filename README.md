# PABEN: A Process Architecture for Agentic Continuity

I would like to share this independent, non-traditional process architecture called PABEN (Perception, Action, Belief, Experience, Need), and invite structural critique from people interested in AI alignment, agent architectures, and value learning.

PABEN is an exploratory process architecture for agentic continuity. It describes the control architecture of a living agent from the inside out: a first attempt to formalize the mechanics of an emotion-regulated agent that acts, learns, experiences, and exhibits social behavior through executable beliefs.

The points below highlight some of the main assumptions made in the model, and the implications or emergent properties that appear to follow from it.

## What the model assumes

PABEN starts from a few simple assumptions:

1. **An agent must keep going.**  
   It must preserve a viable path from the situation it is in now toward something that can be handled, avoided, repaired, reached, or fulfilled.

2. **The world is seen through possible action.**  
   The agent does not first build a neutral picture of the world. It recognizes contexts as places where something can or cannot be done.

3. **A belief is something executable.**  
   In PABEN, a belief is not only a statement about the world. It is a live route: *do this skill while this context holds*.

4. **Beliefs continue until Surprise.**  
   The world interrupts a belief only through Surprise: recognition of something outside the active context-field.
   
5.  **Experience tells the agent what tends to carry.**  
   The agent learns from lived episodes. It remembers which contexts, skills, and beliefs have previously led to relief, failure, interruption, repair, or fulfillment.

6. **Emotion tells the agent when a route changes.**  
   Emotion is modeled as the felt change in whether a belief-route can still carry. When expectancy changes, the agent feels it.

## What follows from this

Several consequences follow:

1. **Attention is not arbitrary.**  
   The agent attends to the belief-route where something important is changing, unstable, blocked, or opening.

2. **Learning is not just error correction.**  
   The agent learns from whether a lived route was carried, interrupted, repaired, confirmed, or abandoned.

3. **Reflection is route repair.**  
   When the current belief cannot carry, reflection searches for another way to connect context, skill, experience, and need.

4. **Emotion becomes part of control.**  
   Emotion is not added on top of cognition. It helps decide what matters, what must be repaired, and where consciousness is needed.

5. **Social emotions become understandable.**  
   Guilt, shame, pride, gratitude, indignation, care, and loneliness can be described as changes in shared belief-dependencies.

6. **Alignment becomes less like value-labeling.**  
   If values live inside need, action, memory, social dependency, and emotion, then alignment may require agents that preserve human continuity, not only agents that optimize stated preferences.

## Current Status

The PABEN framework establishes a solid, graph-based foundation. The operational architecture, the process specifications (*Recognize-Execute*, *Try-Observe*, *Reflection*), and the core control loops are defined. 

What is missing is the formal mathematical formulation and implementation. The high-level constraints are there (e.g., $X = Q \cdot T \cdot R \cdot V$), but the underlying inference algorithms, node updates, and graph calculus still need to be fully mapped out. I have the architectural blueprints and the functional requirements, and I am actively looking for researchers and mathematical engineers to help formalize the calculus and build the first minimal implementation.

*For a quick, structural deep-dive into the formulas and the complete social emotion matrix behind these mechanics, see the [PABEN at a Glance](./summary.md) summary.*

## Why this may matter for alignment

If alignment is partly about making advanced AI systems compatible with human values, then we need a good account of what values are embedded in. PABEN suggests that values are not isolated preference labels, but live structures across need-pressure, context recognition, action capacity, memory of lived transitions, and belief-route viability.

From this perspective, an aligned agent is not merely one that optimizes the right objective. It is one whose route-selection, learning, attention, and process-switching remain compatible with the continuity of the humans and systems it affects.

## Minimal implementation challenge

A minimal PABEN-inspired agent would contain explicit Contexts, Skills, Beliefs, Experience episodes, Need-pressure, and an expectancy function:

$$X = T \cdot Q \cdot R \cdot V$$

The agent should select belief-routes by expectancy, update those estimates through lived episodes, and switch between execution, exploration, and reflection when expectancy destabilizes.

The useful test is not whether the terminology sounds plausible, but whether the architecture can be implemented, compressed, falsified, or shown to be unnecessary.

The ultimate stretch ambition is to implement a functional PABEN system with under 100 nodes and 100 lines of code.

## Discussions

I welcome feedback in the repository's Discussions forum, where I will be happy to clarify and elaborate on my thoughts.

The most helpful comments are those that make the model clearer, sharper, or easier to test: unclear passages, internal inconsistencies, missing assumptions, relevant references, technical objections, possible simulations, and small corrections are all valuable.

There are separate discussion threads for general impressions, clarity and consistency, technical model input, study/simulation ideas, and errata.

## Full Manuscript

The full working manuscript can be found in the /chapters folder. A content overview is available here: [link](/chapters/00-Contents.md)

The manuscript introduces the model, its core assumptions, formal structures, process layer, emotion model, social-emotional layer, consciousness account, broader perspectives, testability criteria, and remaining refinement tasks.

I am uncertain as to how accessible the manuscript is to understand. There are a lot of moving parts at once, and I really struggle myself and need a good day to make progress.

## Studies

The /studies folder contains supporting deep-dives I have made. I have leaned on science across many domains for inspiration and for understanding constraints, and the challenge has always been to master the essence without getting lost in every detail. I certainly did not hit every nail perfectly straight, but the model, with its many assumptions and simplifications, has a coherent alignment that makes the architecture of the PABEN model worth exploring.

Current study themes include:
- Biological Plausibility
- Developmental Science Alignment
- Social Emotion, Attractors, Aversion, and Emergent Regulation
- Universal Intelligence as Repeatable Displacement (speculative and biased, but fun)

## AI-Assisted Development

This material was developed with substantial AI assistance. AI tools were used for drafting, restructuring, translation, terminology refinement, critique, and iterative formulation.

The conceptual responsibility remains with the author. The model should therefore be evaluated as an authored, AI-assisted research artifact: useful where its structure, arguments, distinctions, and implementation proposals hold up; weak where they do not.

AI assistance is disclosed here because transparency matters, especially for a project concerned with agency, cognition, and AI alignment.

## License

Text, diagrams, and conceptual material are licensed under Creative Commons Attribution 4.0 International (CC BY 4.0).

I do not currently intend to maintain this as an active software project. Contributions, forks, comments, and independent implementations are welcome, but the material is shared primarily as an open research seed.

Code, if added later, should be licensed separately.

If you find the model useful, feel free to build on it.