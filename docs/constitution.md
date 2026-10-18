# Project Constitution

## Purpose

This document defines the design and development principles of the application. New features and requirements should align with these principles.

## Principles

### 1. Business Rules Remain in Application Code

Because prompts and language models can fail, behave unexpectedly, or be replaced over time, business rules must be implemented and enforced in application code.

The application remains the authoritative source for enforcing business rules, while the LLM may interpret user requests, assist with decisions, or suggest actions.

### 2. LLMs Must Not Directly Change Application State

Because state-changing operations can affect business data and system behavior, the LLM must never modify application state directly.

The LLM may interpret the user's intent or suggest a state-changing operation, but the application must validate the request, check permissions and business rules, obtain any required user confirmation, and execute the operation itself.
### 3. AI Inputs and Outputs Must Be Validated

Because language models can receive invalid or untrusted data and may produce incorrect or malformed outputs, all AI inputs and outputs must be validated by the application.

The application must ensure that data provided to the LLM is valid and appropriate for the current operation, and that model outputs and tool arguments conform to the expected structure and constraints before they are used.

### 4. Important Behavior Must Be Testable

Because language models can produce inconsistent or incorrect responses, important application behavior must be testable independently of the LLM.

Business rules, permissions, validation, and state-changing operations must be implemented in a way that allows deterministic and repeatable tests.

### 5. State-Changing Operations Require Explicit User Confirmation

Because state-changing operations can have real effects on the system and its data, they must not be executed based only on the LLM's interpretation of user intent.

The application must obtain explicit user confirmation before executing any state-changing operation.