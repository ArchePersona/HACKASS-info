# HACKASS Architecture

HACKASS is the user-facing software-creation program.

It is intentionally separated from the engineering engine and from local-machine execution.

## Responsibility chain

```text
Human
  ↓
HACKASS
  human intent / conversation / product decisions
  ↓
ARCHESTRATOR
  engineering process / plan / work / execution state / verification
  ↓
ROSIE
  local-machine bridge / translation / controlled local action
  ↓
Local machine
  files / repository / shell / tools / runtime
```

## HACKASS

HACKASS owns the human-facing experience.

Its responsibility is to let a person describe software in ordinary language, surface the decisions that materially matter, preserve the user's decision authority, and translate the resulting intent into a form the engineering system can act on.

HACKASS should not require the user to understand ARCHESTRATOR internals, local execution tooling, model-provider mechanics, or deployment architecture.

## ARCHESTRATOR

ARCHESTRATOR is the engineering engine.

Its responsibility begins where product intent becomes engineering work.

It manages concerns such as:

- explicit engineering objectives;
- planning and work decomposition;
- work state;
- execution lifecycle;
- verification;
- continuation and resumability;
- build history; and
- the distinction between what was intended and what actually happened.

ARCHESTRATOR is not the user-facing product and it is not the local-machine bridge.

## ROSIE

ROSIE is the local-machine bridge/runtime.

Its responsibility is locality: translating authorized engineering actions into operations available on the machine where the software actually lives.

The current local action surface includes capabilities such as:

- discovering and searching a workspace;
- inspecting and modifying files;
- inspecting Git state;
- running shell commands; and
- enforcing local approval and workspace boundaries around mutating actions.

ROSIE does not decide the product and does not replace ARCHESTRATOR's engineering process. It provides the controlled path from that process to the local environment.

## Why the separation matters

The stack is designed so each layer can change without requiring the others to become the same thing.

The user can interact with HACKASS without operating an engineering engine.

ARCHESTRATOR can manage engineering work without becoming a web interface.

ROSIE can evolve local-machine access without becoming the product planner or the engineering state machine.

That separation gives HACKASS a path from ordinary human intent to real software while keeping conversation, engineering process, and machine authority distinct.

## Current implementation note

The Google All Things Agentic hackathon implementation uses Google ADK and Gemini in the HACKASS execution path and incorporates pre-existing ARCHESTRATOR execution capabilities. The currently deployed Cloud Run path operates against the workspace available to that deployed runtime.

ROSIE's architectural role is the local-machine bridge. A deployed cloud runtime should not be described as acting on an end user's separate local machine unless a ROSIE local bridge is actually attached and that path has been verified.
