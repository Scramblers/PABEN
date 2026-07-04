# 12. Refinement and Implementation

The PABEN model is presented as an exploratory architecture, not as a finished formal theory. Its value depends on whether it can be refined, constrained, implemented, and possibly refuted. The following themes describe the main work that remains.

### 1. Formal Definition of the Core Structures

The first task is to make the model’s basic structures mathematically precise. Contexts, Skills, Beliefs, Experience episodes, Needs, and Expectancy must be defined in a way that allows computation rather than metaphor.

A minimal formalization should specify what kind of object each domain contains, how elements are created, how they are updated, and how they connect across domains. For example, a Belief should be represented as an action-context route, Experience as lived transitions, and Need as pressure that gives value to possible continuation.

The goal is not to over-formalize too early, but to remove ambiguity where ambiguity prevents implementation.

### 2. Expectancy and the X Function

The expectancy variable, $X$, is central to the model and therefore requires careful refinement. The current formulation is:

$$X=T\cdot Q\cdot R\cdot V$$

where Trustability, Executability, Reachability, and Value estimate whether a belief-route can carry.

The open task is to define how each component is measured or estimated from experience. Trustability should relate to context stability. Executability should relate to skill reliability under context variation. Reachability should relate to whether a route connects from the current context toward a need-relevant outcome. Value should relate to the degree to which the route can regulate, avoid, repair, relieve, or fulfill the active Need-pressure.

A useful implementation must clarify whether these values are probabilities, precisions, weights, learned scores, distributions, or some combination of these.

### 3. Episode Learning and Memory Update

PABEN depends on lived transitions. A candidate episode structure is:

$$Ep_j=(C_{from},B_{lived},N_{felt},C_{to})$$

The implementation task is to define how such episodes are stored, retrieved, strengthened, weakened, generalized, and separated into variants.

A key question is how emotional deformation, $dX$, updates future expectancy. Positive closure should strengthen routes that carried. Negative closure should weaken or mark routes that failed, damaged, or lowered viability. Failed expectation should update the promise-structure: the system learns not only what happened, but what did not happen as expected.

### 4. Process Layer: Recognize-Execute, Try-Observe, and Reflection

The model distinguishes between three major processes: Recognize-Execute, Try-Observe, and Reflection.

Recognize-Execute should describe ordinary flow: the agent recognizes a context, selects a belief, releases a skill, and continues while the belief holds. Try-Observe should describe local variant formation: the agent tests and stabilizes context-skill relations. Reflection should describe higher-level search for viable hooks when no available belief can carry the pressure.

The implementation task is to define process-switching rules. When does the agent continue fluently? When does it explore variants? When does it reflect? When does surprise interrupt? When does an open Need-pressure dominate attention?

These rules should be specified through changes in $T$, $Q$, $R$, $V$, and $dX$ rather than through separate ad hoc controllers.

### 5. Emotion as Control Signal

The model proposes that emotion is the felt deformation of expectancy:

$$dX=X_{after}-X_{before}$$

This must be made operational. An implementation should distinguish between deformations at different process positions: recognition, open promise, realization, and failed realization.

This gives a minimal emotional grammar: surprise at recognition, desire or fear in the open belief, joy or sorrow at realization, disappointment or relief when expected realization fails. Social emotions then require shared belief-dependencies where one agent’s route affects another agent’s $X$.

The refinement task is to define when an emotion-like control state appears, what it does to attention, how it changes process selection, and how it affects learning.

### 6. Social Extension and Multi-Agent Belief-Fields

The social layer remains one of the most important but least implemented parts of the model. Social emotion is proposed to arise when expectancy changes across shared belief-dependencies.

A minimal multi-agent implementation should allow one agent’s action to affect another agent’s context, route, access, or Need-regulation. This would make it possible to model recognition, gratitude, guilt, shame, anger, forgiveness, exclusion, love, and trust as changes in shared expectancy rather than as isolated labels.

The key implementation challenge is to represent shared contexts and dependency. Which beliefs are jointly carried? Which routes depend on another agent? When does another agent become part of one’s own Reachability or Valencability structure?

### 7. Testing, Refutation, and Comparison to Simpler Models

The model should be tested against simpler alternatives. A PABEN-like implementation is only useful if its structural commitments explain or produce behavior that is difficult to obtain from simpler reward-only, policy-only, or prediction-only models.

Important test questions include:

* Does expectancy-based belief-selection produce coherent continuation?
* Does $dX$ improve learning and process-switching?
* Can the model distinguish context failure from skill failure?
* Can it model unresolved promises and persistent emotional tension?
* Can it explain why social recognition, repair, and exclusion matter?
* Can it generate behavior that resembles play, reflection, habit, and surprise without adding separate modules for each?

If the model cannot be implemented, compressed, tested, or distinguished from simpler architectures, it should be revised. If its core mechanisms can be implemented and shown to produce useful behavior, the next task is to make the mathematics more robust.

The purpose of refinement is therefore not to protect the model. It is to expose it. PABEN should become precise enough that others can build it, criticize it, simplify it, or prove that a better architecture exists.
