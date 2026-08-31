# HACKASS

**Hackathon Assassin**

HACKASS was written to destroy the entire premise of hackathons.

Not to win them.
Not to impress them.
Not to perform submission ceremony correctly.

To make the model unnecessary.

## The premise HACKASS attacks

Hackathons exist because software creation has historically been scarce.

Scarce builders.
Scarce technical translation.
Scarce momentum.
Scarce confidence.
Scarce access to people who know how to turn an idea into a working product.

The hackathon model wraps that scarcity in ceremony:

- event windows;
- sponsor stages;
- judging panels;
- demo videos;
- submission gates;
- prize rituals;
- performative innovation language;
- and platform-controlled validation.

That model only matters while ordinary people still need the stage in order to build.

HACKASS removes the stage.

## What HACKASS is

HACKASS is the user-facing software-creation program.

It is the part the human communicates with.

The user does not need to think like an engineer. They describe what they want built in ordinary language. HACKASS carries the conversation, asks for decisions when they materially matter, and turns human intent into software direction.

HACKASS is not the engineering engine and it is not the local-machine execution layer. Those responsibilities are deliberately separated.

## What HACKASS does

HACKASS lets anyone make software by telling it what kind of app they want.

The user does not need to know software development.
The user does not need to know frameworks, data models, deployment paths, hosting rules, or architecture language.
The user does not need to enter a contest so someone else can decide whether their idea deserves to exist.

They describe the app.
HACKASS interviews them when decisions matter.
HACKASS turns intent into requirements, structure, build direction, and implementation work.
HACKASS remains the human-facing surface while the engineering stack underneath it does the specialized work.

## The stack underneath HACKASS

```text
Human
  ↓
HACKASS
  human intent / conversation / product decisions
  ↓
ARCHESTRATOR
  engineering plan / work / execution state / verification
  ↓
ROSIE
  local-machine bridge / translation / controlled local action
  ↓
Local machine
  files / repository / shell / tools / runtime
```

### ARCHESTRATOR

ARCHESTRATOR is the engineering engine.

It turns approved product intent into an inspectable engineering process: planning, work orders, execution, verification, state, continuation, and the record of what actually happened.

### ROSIE

ROSIE is the local-machine bridge/runtime.

Its job is to translate authorized engineering actions into operations the user's machine can actually perform: inspecting and changing files, reading Git state, running commands, and interacting with the local workspace under explicit execution boundaries.

ROSIE does not replace ARCHESTRATOR. ARCHESTRATOR manages the engineering process; ROSIE gives that process a controlled path to the machine where the work lives.

See [Architecture](./docs/ARCHITECTURE.md).

## Why that makes hackathons pointless

The old hackathon promise was simple:

> Come here and build something.

HACKASS changes the promise:

> Stay where you are. Tell me what you need. We build.

Once software creation can begin from ordinary human intent, the hackathon stops being necessary infrastructure.

It becomes pomp and circumstance around a thing people can now do directly.

The banners may remain.
The sponsors may remain.
The judges may remain.
The deadline theater may remain.
The prize table may remain.

But the core function is gone.

Hackathons turned ideas into weekend demos.
HACKASS turns intent into software.

## Origin

HACKASS came from watching real work get filtered out by hackathon ceremony.

The lesson was not that the work was weak.
The lesson was that the filter had become the product.

So HACKASS was built for the projects that should not need permission from a submission gate, a demo format, a sponsor rubric, or a stage manager before becoming real.

You filtered out the wrong builder.

Now the builder is coming for the filter.

## Position

HACKASS is not a hackathon helper.

HACKASS is the thing that makes the hackathon entry format look primitive.

It is software creation without asking the hackathon model for access, validation, timing, or permission.

## Documentation

Supporting documentation is available in [`docs/`](./docs/):

- [Premise](./docs/PREMISE.md)
- [Product](./docs/PRODUCT.md)
- [Workflow](./docs/WORKFLOW.md)
- [Architecture](./docs/ARCHITECTURE.md)
- [Market Attack](./docs/MARKET_ATTACK.md)
- [IP and Licensing](./docs/IP_AND_LICENSING.md)

## License

For now, HACKASS keeps the IP.

This repository is currently proprietary. Public visibility does not grant permission to copy, modify, distribute, host, deploy, train on, or create derivative works from the project.

See [`LICENSE`](./LICENSE).

## Public thesis

HACKASS exists to kill the reason hackathons matter.

If anyone can describe the app they want and be walked toward working software, then the hackathon is no longer the place where software becomes possible.

It is just a stage.

HACKASS makes the stage pointless.
