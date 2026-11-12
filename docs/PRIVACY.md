# Privacy

TestFlow Recorder is a QA automation tool that operates on web applications explicitly selected by the user.

## What the extension may process

Depending on enabled features, TestFlow may process:

- page structure required for locator generation;
- user-triggered browser interactions;
- navigation context;
- diagnostic metadata;
- screenshots used as test evidence;
- recorded test values.

## Sensitive values

Teams should avoid recording real production credentials or personal data.

TestFlow provides privacy-oriented controls such as custom sensitive selectors:

```css
[data-sensitive],[data-private]
```

These selectors can be adapted to the application under test.

## Screenshots

Before evidence screenshots are captured, TestFlow temporarily hides its own UI overlays so that the screenshot represents the application under test.

## Data usage

TestFlow Recorder is intended for software testing workflows.

It is not designed for advertising, profiling, or unrelated browsing analytics.

## Recommended practice

Use:

- dedicated test accounts;
- synthetic data;
- non-production environments;
- masked credentials;
- privacy selectors;
- sanitized evidence before sharing reports.

---

**Developed by aematosy**
