# Workflow

HACKASS turns ordinary intent into software work without asking the user to think like an engineer.

It begins by letting the user say what they want built.

## 1. Intent capture

The user describes the app in plain language.

Examples:

- I need an app for booking local services.
- I need a private dashboard for my research.
- I need a tool that helps teachers manage student check-ins.
- I need a marketplace for a niche community.
- I need a simple internal tool for tracking evidence, decisions, and work history.

The first input does not need to be complete.

## 2. Decision interview

HACKASS asks questions only when the answer changes the product, workflow, architecture, cost, scope, or user experience.

It does not drown the user in software jargon.

It pulls out the decisions that matter.

## 3. Product shaping

HACKASS identifies:

- the users;
- the primary job to be done;
- the main workflows;
- the data involved;
- the required screens;
- the risky assumptions;
- the first useful version;
- the boundaries between must-have and later.

## 4. Engineering handoff

Once the material product decisions are established, HACKASS hands the approved build intent to ARCHESTRATOR.

ARCHESTRATOR is the engineering engine. It owns the structured build process around that intent: planning, work organization, execution state, verification, continuation, and the record of what happened.

HACKASS remains the user-facing surface. The user should not have to manually operate ARCHESTRATOR in order to use the product.

## 5. Local execution

When engineering work must reach the user's machine, ROSIE provides the local bridge/runtime.

ROSIE translates authorized engineering actions into operations available on the local machine, including:

- workspace discovery;
- file inspection and modification;
- Git inspection;
- shell execution; and
- other bounded local actions exposed through its tool layer.

The responsibility split is deliberate:

```text
HACKASS      understands and carries human intent
ARCHESTRATOR manages the engineering process
ROSIE        translates authorized work into local-machine action
```

## 6. Software path

The outcome is not a plan sitting in a conversation.

The outcome is movement from human intent through engineering work toward running software.

```text
Human intent
  ↓
HACKASS
  ↓
ARCHESTRATOR
  ↓
ROSIE
  ↓
Local machine
  ↓
Working software
```

The user does not need a hackathon stage to begin.

The user needs a system that can carry intent all the way into software.

That is HACKASS.
