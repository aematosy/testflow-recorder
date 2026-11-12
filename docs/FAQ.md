# Frequently Asked Questions

## Is TestFlow Recorder open source?

No. This repository contains public documentation, guides, screenshots, and release information. The implementation source code is not published.

## What is the JSON used for?

The JSON is the portable representation of the recorded test flow.

It can be used for review, replay, transformation, automation generation, and integration with framework-specific tooling.

## Does it support Playwright?

Yes. TestFlow supports Playwright-oriented mappings for TypeScript and Python.

## Does it support pytest?

Yes. The Playwright/Python output is suitable for pytest-based automation projects.

## Does it support Serenity?

Yes. TestFlow supports Serenity BDD Screenplay / Java concepts.

## Why doesn't TestFlow record every keyboard event?

Because raw event capture creates noisy and brittle tests. TestFlow focuses on keyboard interactions that contribute to test intent.

## Why doesn't TestFlow keep every hover?

A hover is retained only when it contributes to a meaningful downstream action.

## Why is an assertion inserted before the action?

Because the precondition should be validated before performing the action.

## Can I reorder multiple steps?

Yes. Multiple selected steps can be moved while preserving their relative order.

## Can TestFlow enable Incognito automatically?

No. Chrome requires the user to explicitly enable extension access to Incognito mode.

## Does the SPY support iframe and Shadow DOM?

The locator model includes context for complex DOM scenarios. Exact support can depend on the application structure and browser constraints.

## What if no unique locator is found?

Try inspecting the parent/child semantic element or use a manual locator as a last resort.

## Are screenshots clean?

The extension hides its own overlays before evidence capture so TestFlow controls do not appear in the screenshot.

---

**Developed by aematosy**
