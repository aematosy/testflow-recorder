# Public Architecture Overview

This document describes TestFlow Recorder at a conceptual level without exposing proprietary implementation details.

## Major product areas

### Recorder

Captures user-intent events and normalizes them into a portable flow model.

### Locator analysis

Evaluates multiple locator strategies and ranks candidates according to stability and uniqueness.

### Context resolution

Tracks page, iframe, and DOM context required to replay or export an action.

### Element Inspector

Allows a user to inspect the DOM independently from the main recording flow.

### Runner

Provides review, ordering, assertion management, locator selection, skipping, waits, and isolated replay.

### Evidence

Generates screenshots and execution artifacts.

### Export model

The portable flow can be interpreted by framework-specific automation tooling.

## Design principle

The public JSON/flow representation is the contract between recording and framework-specific automation.

This public repository intentionally does not contain proprietary extension source code.

---

**Developed by aematosy**
