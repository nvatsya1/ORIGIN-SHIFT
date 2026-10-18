# ORIGIN-SHIFT
# ORIGIN SHIFT
### See how your thinking changes.

**ORIGIN SHIFT is an AI-powered belief-tracking tool designed to make changes in human reasoning visible, traceable, and open to scrutiny.**

AI systems increasingly influence how people interpret information, evaluate arguments, and form opinions. Yet most AI interfaces focus on the answer, not on how interacting with that answer changes the person receiving it.

ORIGIN SHIFT explores a different approach: instead of simply recording what an AI says, it tracks how a person's beliefs evolve throughout an interaction.

## The Problem

When someone interacts with an AI system, their initial assumptions can shift as they encounter new information, persuasive arguments, and generated explanations.

However, the process is often difficult to reconstruct afterward.

- **Invisible belief changes:** People may not recognize which parts of a conversation changed their perspective.
- **Unclear claim origins:** It can be difficult to distinguish an externally supported fact from an AI-generated assertion or an inference.
- **Misplaced confidence:** A person may become more confident in a conclusion without receiving stronger evidence.
- **Missing reasoning history:** Traditional chat histories preserve messages but rarely provide a structured account of how beliefs changed.

The result is a gap between what people believe and their ability to explain why they believe it.

## The Solution

ORIGIN SHIFT turns an AI-assisted reasoning session into a structured, inspectable record of belief change.

Its central concept is the **Belief Transition Record**, which maps the progression from an initial belief to a revised position, connecting influential claims, supporting evidence, reasoning steps, and changes in confidence.

Rather than treating a changed opinion as a simple before-and-after comparison, ORIGIN SHIFT aims to reconstruct the transition itself.

## How It Works

### 1. Establish a baseline
The user records an initial belief, position, or hypothesis, along with their confidence in it.

### 2. Introduce new information
The user examines a question, argument, or topic through an AI-assisted interaction.

### 3. Identify influential claims
The system extracts relevant claims from the interaction and distinguishes claims requiring external verification from evidence and reasoning presented in the conversation.

### 4. Trace the transition
The system connects the original belief to the claims and evidence associated with a change in position. It identifies which parts of the reasoning chain are supported, uncertain, or unverified.

### 5. Examine the cognitive difference
The user compares their initial and revised positions, including changes in confidence, assumptions, and supporting reasons.

### 6. Review the Belief Transition Record
The resulting record provides an inspectable explanation of what changed, what may have influenced the change, and where uncertainty remains.

## Core Features

- **Belief Baseline:** Capture an initial position and its associated confidence.
- **Claim Lineage:** Trace claims to their originating conversation passages and any available supporting sources.
- **Belief Transition Record:** Represent the relationship between initial beliefs, influential claims, evidence, reasoning, and revised beliefs.
- **Cognitive Diff:** Compare an initial position with a revised one to surface changes in conclusions, assumptions, and confidence.
- **Confidence–Evidence Gap:** Highlight situations in which confidence changes without a corresponding increase in verified evidentiary support.
- **Evidence and Uncertainty Mapping:** Distinguish verified evidence, unsupported assertions, inferences, and unresolved questions.
- **Interactive Exploration:** Let users inspect individual claims and understand how they relate to a broader change in belief.

Feature availability depends on the implemented version. Claims, sources, and inferred relationships should remain distinguishable rather than being presented as equally certain.

## What Makes ORIGIN SHIFT Different?

Most AI tools optimize for producing an answer. ORIGIN SHIFT focuses on understanding the effect of that answer on the person receiving it.

Its central innovation is the shift from **answer generation to belief-transition analysis**.

The project brings together ideas from cognitive science, explainable AI, and evidence-aware reasoning to investigate a consequential question:

**Can we make the process of changing our minds as inspectable as the information that prompted the change?**

ORIGIN SHIFT does not assume that changing one's mind is inherently good or bad. It aims to make the transition more transparent so that people can evaluate their own reasoning rather than accepting a conclusion simply because it feels persuasive.

## Intended Applications

- **Education:** Help students examine how evidence changes their understanding of a topic.
- **AI literacy:** Make the influence of AI-generated claims easier to inspect.
- **Research:** Support structured reflection on evolving hypotheses and interpretations.
- **Decision-making:** Document the reasoning behind consequential changes in position.
- **Critical thinking:** Encourage users to distinguish confidence, plausibility, and evidentiary support.

## Technology and Architecture

ORIGIN SHIFT is designed as an end-to-end proof of concept.

The intended architecture separates the user interface from the analysis layer:

1. **Frontend:** Collects initial beliefs, presents the analysis workflow, and visualizes belief transitions.
2. **Analysis backend:** Processes user-provided interactions and returns structured claims, belief comparisons, evidence assessments, and uncertainty indicators.
3. **AI analysis layer:** Supports claim extraction, semantic comparison, and proposed relationships between claims and changes in belief.
4. **Evidence handling:** Preserves available source references and distinguishes externally verified information from unsupported or unverified claims.
5. **Belief record:** Structures the analysis into a record that users can inspect.

The implementation should clearly distinguish model-generated interpretations from independently verified evidence. A claim appearing in a conversation is not, by itself, proof that the claim is true or that it caused a change in belief.

**Implementation note:** Update this section with the actual frameworks, AI provider, database, and deployment configuration used by the repository.

## Project Scope

The initial version focuses on demonstrating one complete workflow: capture an initial belief, analyze an AI-assisted interaction, compare the resulting positions, and display an inspectable Belief Transition Record.

The proof of concept should prioritize a functional end-to-end experience over an expansive feature set.

Future directions could include longitudinal belief histories, comparisons across multiple conversations, richer evidence graphs, and research-oriented tools for examining human–AI interaction.

## Responsible Design

ORIGIN SHIFT is an exploratory reasoning aid, not a mind-reading system.

A difference between two statements does not establish why a person's belief changed. The system should describe observed differences and plausible influences without claiming certainty about internal mental processes.

It should also:
- Preserve uncertainty when the evidence is incomplete.
- Avoid treating confidence as a measure of truth.
- Distinguish correlation, plausible influence, and demonstrated causation.
- Make unsupported claims and missing evidence visible.
- Allow users to challenge or correct the system's interpretation.

## Getting Started

Clone the repository:

```bash
git clone <YOUR_GITHUB_REPOSITORY_URL>
cd origin-shift
```

Install the dependencies using the package manager and instructions specified by the project.

Configure the required environment variables for the selected AI provider and backend, if applicable. Keep API keys in environment variables or an untracked `.env` file. Never commit credentials to GitHub.

Start the frontend and backend using the repository's development scripts.

**Setup instructions should be finalized once the actual project structure and package scripts are confirmed.**

## Project Status

ORIGIN SHIFT is being developed as a hackathon proof of concept. Its goal is to demonstrate how AI-assisted interactions can be transformed into structured, evidence-aware records of belief change.

## The Big Idea

We can preserve conversations. We can evaluate claims. We can measure confidence.

But can we trace the path from one belief to another?

**ORIGIN SHIFT is an attempt to make that path visible.**
