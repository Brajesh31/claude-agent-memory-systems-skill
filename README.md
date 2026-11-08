# claude-agent-memory-systems-skill

A Claude Code skill for designing memory architectures that help AI agents retain, organize, and retrieve useful information over time.

## Overview

Agent memory is more than persistent storage. A system may store large amounts of information and still fail if it cannot retrieve the right knowledge at the right moment.

This skill covers memory types, storage choices, chunking, embeddings, retrieval, temporal relevance, conflict resolution, and evaluation.

## Memory Types

| Type | Purpose |
|---|---|
| Short-term | Current interaction and active context |
| Working | Information needed for the current task |
| Episodic | Records of events and past interactions |
| Semantic | Stable facts and concepts |
| Procedural | Reusable workflows and instructions |
| Long-term | Durable knowledge across sessions |

Not every agent needs every memory type. Select based on the task, retention period, and retrieval requirements.

## Main Capabilities

- Design short-term and long-term memory.
- Choose memory representations and storage.
- Plan chunking and metadata.
- Select embedding and retrieval strategies.
- Rank results by relevance and recency.
- Handle stale and conflicting information.
- Control memory formation and decay.
- Evaluate retrieval quality.
- Diagnose memory-related failures.

## Installation

```bash
git clone https://github.com/Brajesh31/claude-agent-memory-systems-skill.git ~/.claude/skills/agent-memory-systems
```

## Usage

Invoke the skill when designing or improving agent memory:

```text
/agent-memory-systems
```

Provide the agent's use case, information types, expected retention, query patterns, data volume, and privacy constraints.

## Recommended Design Workflow

1. Identify what the agent needs to remember.
2. Separate temporary context from durable knowledge.
3. Choose memory types based on information use.
4. Define write and update policies.
5. Design chunking and metadata together.
6. Select storage and retrieval mechanisms.
7. Rank results using relevance and temporal context.
8. Handle stale, duplicate, and contradictory records.
9. Evaluate retrieval with realistic queries.
10. Monitor memory quality as the system evolves.

## Retrieval Quality

Evaluate whether the system retrieves:

- The correct information.
- Enough context to interpret it.
- The most relevant and current version.
- The right information for the current task.
- No unnecessary sensitive or unrelated records.

Measure retrieval quality independently from answer generation. Otherwise, a retrieval failure may be mistaken for a model reasoning problem.

## Common Failure Modes

- Storing everything without a retention policy.
- Using one memory type for every kind of information.
- Creating chunks that lose important context.
- Relying on embeddings without useful metadata.
- Ignoring recency and version conflicts.
- Retrieving too much context.
- Failing to evaluate retrieval with real queries.

## Repository Contents

- `SKILL.md`: Main agent memory architecture guidance.
- `README.md`: Memory types, design workflow, and retrieval checklist.

## Practical Principle

A memory system succeeds when it retrieves useful knowledge at the right time. Storage capacity alone is not a measure of intelligence.
