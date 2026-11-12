# Framework Support

TestFlow Recorder stores a framework-neutral flow model and exposes enough metadata to map recorded actions into multiple automation stacks.

## Serenity BDD Screenplay / Java

Typical mappings:

| TestFlow action | Serenity concept |
|---|---|
| click | `Click.on(...)` |
| type | `Enter.theValue(...).into(...)` |
| select | `SelectFromOptions...` |
| right click | `RightClick.on(...)` |
| hover | `MoveMouse.to(...)` |
| assertion | `Ensure.that(...)` |

## Playwright / TypeScript

Typical mappings:

```ts
await locator.click();
await locator.fill(value);
await locator.hover();
await locator.selectOption({ label: value });
await expect(locator).toBeVisible();
```

## Playwright / Python

Typical mappings:

```python
locator.click()
locator.fill(value)
locator.hover()
locator.select_option(label=value)
expect(locator).to_be_visible()
```

## pytest

TestFlow does not require a specific pytest project structure.

The exported Playwright/Python representation can be integrated into:

- pytest fixtures;
- Page Object models;
- Screenplay-like Python architectures;
- custom flow/service layers.

## Important

TestFlow Recorder is intended to accelerate automation design, not replace engineering review.

Before committing generated automation:

1. review locators;
2. remove redundant actions;
3. move reusable logic into framework abstractions;
4. parameterize test data;
5. align waits and assertions with application behavior.

---

**Developed by aematosy**
