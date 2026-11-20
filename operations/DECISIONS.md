# Architecture Decisions

## DEC-001 — Git is the canonical coordination record
**Date:** 2026-11-20  
**Status:** ACCEPTED

Project state, tasks, decisions, and verification evidence live in version control. Chat transcripts are transient interfaces, not authoritative project state.

## DEC-002 — Portable core, thin agent adapters
**Date:** 2026-11-20  
**Status:** ACCEPTED

Maintain one shared operating contract and skill source. Add only the minimum adapter required by each agent's actual supported mechanism. Do not assume one SKILL.md installs natively in every AI product.

## DEC-003 — No false synchronization claims
**Date:** 2026-11-20  
**Status:** ACCEPTED

A repository connection, file access, MCP tool, or browser capability must be tested independently. An agent is CONNECTED only after it reads canonical state and completes a verified write cycle.
