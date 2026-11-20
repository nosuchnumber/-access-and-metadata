# FML AI Operating System

**Status:** FOUNDATION / SPECIFIED  
**Owner:** NoSuchNumber.99  
**Organization:** Fine-Mind-Love Entertainment (FML)

A shared operating protocol for AI agents and development environments working across FML, VOIDCORE, audio engineering, software, and business operations.

## Core rule

The repository is the canonical coordination record. Agents read current state before acting, claim a bounded task, produce changes or evidence, verify them, and update state. The operator should not have to shuttle summaries between models.

## Architecture

- `state/`: authoritative system and project state.
- `operations/`: task queue, decisions, technical log, and handoff records.
- `protocols/`: shared agent contract and verification rules.
- `skills/fml-operator/`: portable operator skill source.
- `adapters/`: thin instructions for individual agent environments.

## Agent compatibility

The protocol is shared; installation is adapter-specific. Claude Code, Gemini CLI, Codex/ChatGPT, Antigravity, Manus, and Opal must not be described as connected until their actual repository/filesystem integrations are configured and tested. A shared GitHub repository alone does not create live synchronization with every product.

## Operating states

PROPOSED → SPECIFIED → BUILDING → TESTING → VERIFIED → DEPLOYED  
Use PARKED for intentionally paused work. Never mark a task complete without an artifact or verification evidence.

## Security

Never commit credentials, API keys, private audio, unreleased source material, personal location data, or machine-specific secrets. Keep private operational evidence in approved private storage.

## First integration milestone

Prove one end-to-end cycle: read state → claim task → change a real artifact → run a verification → commit evidence → update state. Then add agent adapters one at a time.
