# Spec-Driven AI Publishing Assistant

A learning and portfolio project exploring how to build an AI-assisted content publishing system using **Spec-Driven Development (SDD)**.

The project combines traditional software engineering practices with LLM-based capabilities while keeping business rules, permissions, and state-changing operations under application control.

> **Status:** Work in progress — currently in the specification and design phase.

## Project Goal

The goal is to design and implement a small content publishing system where users can interact with an AI assistant using natural language.

The assistant will eventually be able to help users:

- retrieve blog post information;
- review whether a post is ready for publication;
- produce structured review results;
- suggest application tool calls;
- interact with selected capabilities through MCP.

The LLM is **not** treated as the authority for business decisions.

Operations such as publishing must remain protected by deterministic application rules, authorization checks, validation, and user confirmation.

## Engineering Focus

This project is intended to explore and demonstrate concepts including:

- Spec-Driven Development (SDD)
- Business rule enforcement
- Application boundaries
- Structured LLM outputs
- Prompt engineering
- Context engineering
- Tool calling
- Human confirmation for state-changing operations
- Authorization and permission checks
- Idempotency and safe retries
- Model Context Protocol (MCP)
- Prompt injection resilience
- Automated testing

## Development Process

The project follows an SDD-oriented workflow:

```text
Constitution
    ↓
Specify
    ↓
Clarify
    ↓
Plan
    ↓
Tasks
    ↓
Analyze
    ↓
Implement
    ↓
Test
```

Important architectural and behavioral decisions are documented before implementation.

Changes to important requirements should first be reflected in the specification rather than being introduced directly in code.

## Repository Structure

The repository is currently in its specification phase.

```text
docs/
├── constitution.md
├── specification.md
└── clarifications.md
```

The application and test project structure will be defined after the planning phase.

## Technology

The implementation is planned around **C# and .NET**.

Additional technologies and architectural choices will be documented as they are decided during the planning process.

## Origin

This project is being developed as part of a software engineering and Generative AI learning exercise.

The original assignment can be found here:

https://github.com/oroumand/SoftwareEngineering-GenAI-0505/blob/main/Session-05/Homework/homework.md

The analysis, specifications, architectural decisions, implementation, tests, and project documentation in this repository are my own work.

## Current Progress

- [ ] Constitution
- [ ] Specification
- [ ] Clarification
- [ ] Implementation Plan
- [ ] Task Breakdown
- [ ] Specification Analysis
- [ ] Core Application
- [ ] Automated Tests
- [ ] Structured Output
- [ ] LLM Integration
- [ ] Tool Calling
- [ ] Confirmation Workflow
- [ ] Safe Retry / Idempotency
- [ ] MCP Server
- [ ] MCP Resource
- [ ] Prompt Injection Scenario
- [ ] Final Demo
