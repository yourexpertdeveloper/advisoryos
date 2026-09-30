# AdvisoryOS Architecture

## Overview

AdvisoryOS is designed as a Telegram-first AI operating system for advisory work.

The architecture is intended to combine:

- Chief of Staff orchestration
- Specialist agents
- Knowledge retrieval
- Document analysis
- Workflow automation
- Independent review
- Human approval controls

## Core Flow

A simplified request flow is:

User
↓
Telegram
↓
Chief of Staff / Request Router
↓
Task Classification
↓
Retrieval / Specialist Workflow
↓
Analysis
↓
Review where required
↓
Final Response or Deliverable

## Retrieval Strategy

The preferred retrieval hierarchy is:

1. Direct reference
2. Deterministic search
3. Semantic/QMD search
4. Agent reasoning

This approach is intended to reduce unnecessary model usage and improve reliability.

## Human Approval

The system can prepare and analyse information autonomously, but external actions require human approval.

Examples include:

- Sending
- Publishing
- Deleting
- Transferring
- Submitting
- Executing external commitments

## Development Status

This architecture is under active development and will evolve as additional workflows and reliability improvements are implemented.
