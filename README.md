# Agent Memory Systems Skill

A Claude skill focused on the architecture of memory for intelligent agents. It explains how short-term, working, episodic, semantic, procedural, and long-term memory fit into an agent system, with particular attention to retrieval quality.

## What This Skill Covers

- Choosing memory types for different information and tasks.
- Designing short-term and long-term memory components.
- Selecting vector stores and retrieval approaches.
- Applying chunking strategies that support useful retrieval.
- Thinking about memory formation, decay, and conflict handling.
- Avoiding common failures such as storing everything forever or using one memory type for all data.

## Repository Structure

- `SKILL.md`: Skill definition, capabilities, design patterns, anti-patterns, and common memory-system pitfalls.
- `LICENSE`: MIT License for this repository.

## Core Idea

Persistent storage alone does not make an agent remember well. The system must retrieve the right information at the right time. Chunking, embeddings, metadata, temporal relevance, and retrieval evaluation all affect whether stored knowledge is useful during a later interaction.

## When to Use It

Use this skill when designing an agent memory architecture, comparing retrieval strategies, diagnosing inconsistent answers, or deciding how to represent different kinds of knowledge. It is also useful when reviewing a system that stores substantial information but retrieves irrelevant or incomplete context.

## Getting Started

1. Add the skill to a Claude-compatible skills environment.
2. Describe the agent's memory requirements and the information it needs to retain.
3. Select memory types based on usage and lifetime.
4. Design chunking and retrieval together, then test retrieval against realistic queries.
5. Review memory quality over time and address conflicts, staleness, and irrelevant results.

## License

Released under the MIT License. See [LICENSE](LICENSE) for details.
