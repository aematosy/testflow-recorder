# TestFlow Recorder

TestFlow Recorder is a browser extension for capturing, inspecting, refining, and replaying web UI test flows.

It combines interaction recording, resilient locator discovery, Object Spy, assertions, isolated execution, and automation-ready exports in a single QA workflow.

## Features

- Record web UI interactions
- Object Spy for element inspection
- Resilient locator discovery
- Multiple locator alternatives
- Exact unique-target validation
- Semantic and structural locator strategies
- Assertions
- Flow editing and step reordering
- Skip or remove actions before execution
- Global and per-action timeouts
- Editable runtime test data
- Isolated replay
- HTML execution reports
- Flow JSON export and import
- iframe support
- Open Shadow DOM support
- Closed Shadow DOM capture support
- English and Spanish UI

## Automation-ready output

TestFlow Recorder exports structured flow information designed for downstream automation workflows.

Initial target frameworks:

- Playwright + TypeScript
- Serenity BDD + Screenplay + Java

The exported flow contains functional steps, semantic target information, locator alternatives, execution context, assertions, iframe information, Shadow DOM paths, and framework-oriented metadata.

## Locator strategy

TestFlow Recorder does not select a locator simply because it works once.

Recommended locators are evaluated using semantic identity, stability, execution context, and exact target matching.

Executable locator candidates must resolve to exactly one target.

The locator engine can use strategies based on:

- stable attributes
- accessible roles and names
- labels
- test identifiers
- names and placeholders
- stable links
- visible semantic text
- CSS selectors
- XPath
- parent/child relationships
- ancestor/descendant relationships
- sibling relationships
- iframe context
- Shadow DOM context

Positional selectors and transient UI state are avoided when a more stable alternative is available.

## Object Spy

Object Spy allows elements to be inspected without modifying the recorded flow.

It provides:

- recommended locator
- alternative locators
- locator copy
- assertion creation
- action creation
- pause/resume inspection
- manual navigation while paused

## TestFlow Runner

The Runner provides a dedicated workspace for reviewing and executing a recorded flow.

Before execution you can:

- edit runtime input data
- select execution locators
- provide a manual locator when necessary
- add assertions
- skip actions
- remove selected actions
- configure maximum wait times

Execution results include passed, failed, skipped, and not-executed actions.

## Reports

TestFlow Recorder generates a standalone HTML execution report containing:

- execution summary
- progress
- passed/failed/not-executed metrics
- action results
- locator information
- assertion results
- failure diagnostics
- execution evidence

## Installation

Download the latest packaged release from the repository Releases section.

This repository distributes the packaged extension only. Development source code and internal implementation are maintained separately.

## Current release

**TestFlow Recorder 3.0.9**

The packaged extension is available under `releases/`.

SHA-256 checksums are provided for release verification.

## Security

Sensitive runtime values such as passwords are not exported in plain text.

Packaged releases do not include development source files, internal tests, source maps, or private signing material.

## Project status

TestFlow Recorder is currently under active development and evaluation as a QA automation accelerator.

---

© 2026 Adrian Matos
