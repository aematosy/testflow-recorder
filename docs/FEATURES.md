# Feature Reference

## Recorder

Captures meaningful test actions while filtering low-value browser noise.

Supported categories include:

- click
- type
- select
- navigation
- double click
- right click
- keyboard shortcuts with observable effect
- hover with downstream intent
- assertions

## Element Inspector

- exact element inspection
- parent inspection
- primary locator
- alternative locators
- copy locator
- add assertion
- add action
- minimize/restore locator panel
- iframe awareness
- Shadow DOM awareness

## Locator engine

Candidate strategies include:

- stable test attributes
- stable IDs
- ARIA role and accessible name
- labels
- name
- placeholder
- normalized text
- semantic CSS
- parent/child relations
- sibling relations
- XPath fallback
- href / alt / src strategies for links and images

## Assertions

Context-sensitive assertion catalog based on target element.

## Runner

- flow review
- locator selection
- manual locator
- assertions
- skip
- wait configuration
- delete
- multi-select
- move up/down
- automatic renumbering
- isolated execution
- progress state
- evidence

## Evidence

- screenshots
- HTML execution report
- JSON flow
- diagnostic metadata

## Privacy

- custom CSS selectors for sensitive data
- masking-oriented workflow
- extension overlays hidden before screenshots

## Internationalization

English and Spanish interfaces are maintained in parallel.

## Framework interoperability

Supported target families:

- Serenity Screenplay / Java
- Playwright / TypeScript
- Playwright / Python
- pytest integration
