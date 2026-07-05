# Browser Bug Test Artifact Checklist

A screenshot shows where the bug ended. A test artifact shows what happened.

Use this when a QA, support, product, or automation report needs to be trusted by engineering without another round of questions.

## Minimum test artifact

1. **Path**
   - URL or route
   - account/workspace state
   - browser/device/viewport
   - feature flags or environment

2. **Intent**
   - what the user/test/agent tried to do
   - expected result
   - why this flow matters

3. **Action**
   - exact element or locator
   - click/type/navigation/upload/download action
   - timestamp and step order

4. **Before state**
   - visible page state
   - relevant DOM/value state
   - console/network state if useful

5. **Settlement**
   - did the page process the action?
   - did focus move?
   - did the input value match?
   - did navigation finish?
   - did the relevant network request complete?

6. **Delta**
   - what changed after the action?
   - URL, text, element count, DOM state, console errors, network, storage, download, screenshot, trace
   - if nothing changed, record the no-op as a fact

7. **First failure signal**
   - the earliest point expected and actual diverged
   - not just the final broken screen

8. **Shareable artifact**
   - replay, screenshot, trace, HAR, console slice, input diff, or step log
   - enough context for someone else to inspect without a live screenshare

## Good report shape

```text
Expected: [what should have happened]
Actual: [what happened]
First failure signal: [earliest divergence]
Path: [route/account/env/browser]
Steps: [numbered actions]
Evidence: [replay/screenshot/trace/network/console]
State before action: [what the page showed]
State after action: [what changed or did not change]
```

## One-line rule

If engineering has to ask “what happened before the screenshot?”, the report is missing the test artifact.

Samelogic gives teams test artifacts for important browser work: replayable proof of the path, state, element, action context, and first failure signal.
