# PABEN: A Process Architecture for Agentic Continuity

PABEN is an exploratory process architecture for agentic continuity. The model proposes that an agent can be understood as a system that preserves viable continuation through five interacting domains: Perception, Action, Belief, Experience, and Need.

PABEN describes the control architecture of a living agent from the inside out. It is a formalization of the mechanics behind an emotion-regulated agent that acts, learns, experiences, and exhibits social behavior entirely through executable beliefs. By implementing a set of very specific architectural design choices, a series of highly sophisticated, emergent capabilities naturally unfold.

## Architectural Design Choices (The Core Premises)
The 5 foundational constraints built into the agent's processing engine:

* **Agent-Centric Predictive Vision (Affordances)**: The system parses environment data exclusively as relational action-capabilities mapped to internal needs, bypassing static object classification.
* **Multiplicative Expectancy Function ($X$)**: Predictability is calculated as the product of four conditional probabilities: Executability ($Q$), Trustability ($T$), Reachability ($R$), and Valencability ($V$).
* **Emotions as a Dynamic Vector Signal ($dX$)**: "Emotions" are defined as the time-derivative of the expectancy function, representing a high-density signal carrying valence, amplitude, and causal attribution.
* **Attentional Allocation through Max/Min Friction**: Consciousness operates as a resource-allocation mechanism, locking attention onto beliefs with the highest variance ($\text{Max}\vert{}dX\vert{}$).
* **Primary Social Imbrication (Shared-Belief Bootstrapping)**: The agent initiates with shared-beliefs and universal animism, learning to differentiate itself from the environment rather than building social structures from scratch.

## Emergent Capabilities (The Computational Payoff)
The 5 high-value behaviors that emerge organically from the engine:

* **Automated Attention Economy**: Static variables decay into the background through the Trustability coefficient, while volatile vectors are automatically identified as intentional agents.
* **Structural Empathy Engine**: Human social emotions (Guilt, Indignation, etc.) emerge natively when the $dX$ vector registers that an external agent caused a systemic disruption.
* **Autonomous Coping Loops (Social Homeostasis)**: Social-emotional vector states trigger stabilization algorithms, deploying behavioral patches like Serving or Bonding to maintain equilibrium.
* **Organic Cognitive Ontogeny (Developmental Scaling)**: The architecture allows for natural maturation, scaling from externally regulated nodes to internalized agency.
* **Fractal Algorithmic Scalability**: The core design blocks scale fluidly from low-level sensory-motor navigation to macro-level multi-agent coordination based on continuity-preserving displacement.

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

I am uncertain as to how accesible the manuscript is to understand. There are a lot of moving parts at once, and I really struggle myself and need a good day to make progress.

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