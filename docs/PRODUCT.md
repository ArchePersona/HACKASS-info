# Product

HACKASS lets anyone make software by telling it what kind of app they want.

The user does not need to know software development.
The user does not need to know frameworks.
The user does not need to know data models.
The user does not need to know deployment.
The user does not need to know how to translate a product idea into engineering language.

HACKASS handles the human-facing translation layer.

## What HACKASS is

HACKASS is the user-facing software-creation program for people who know what they want built but do not know how to build it.

It is the part the user communicates with.

It is not the engineering engine, the local-machine runtime, or a generic coding model.

## What HACKASS does

HACKASS can:

- receive an app idea in ordinary language;
- ask clarifying questions when decisions matter;
- identify users, workflows, constraints, and outcomes;
- turn intent into product requirements;
- shape the build direction;
- preserve the user's control over material decisions;
- hand approved engineering intent into the execution stack; and
- keep the user-facing experience centered on what they want rather than how software is implemented.

## The system beneath the product

HACKASS deliberately separates the user experience from engineering and machine execution.

```text
Human
  ↓
HACKASS
  intent / conversation / product decisions
  ↓
ARCHESTRATOR
  engineering process / work state / execution / verification
  ↓
ROSIE
  local-machine bridge / controlled local actions
  ↓
Local workspace
```

**ARCHESTRATOR** is the engineering engine. It manages the structured process around building software.

**ROSIE** is the local-machine bridge/runtime. It translates authorized actions into file, Git, shell, and workspace operations on the machine where the work lives.

That separation matters: the user should not have to operate an engineering engine or a terminal in order to make software.

## User promise

Tell it what app you want.

It walks you into software.

No stage required.
