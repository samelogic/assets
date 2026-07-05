# Can't Reproduce Bug Report Template

Use this when a browser bug gets stuck because the report shows the final broken screen but not the trail that got there.

## Copy/paste template

```text
Title: [area] [short failure]

Expected:
[what should have happened]

Actual:
[what happened]

First failure signal:
[the earliest point where expected and actual split]

Path:
- URL/route:
- account/workspace state:
- environment:
- browser/device/viewport:
- feature flags/data setup:

Steps:
1.
2.
3.

Action before failure:
[click/type/navigation/upload/download/submit]

State before action:
[what the page showed before the failing action]

State after action:
[what changed, or what did not change]

Evidence:
- screenshot:
- screen recording/replay:
- console errors:
- network request/response:
- trace/HAR/logs:

Reproduction notes:
- happens every time / sometimes / once:
- tried again and got:
- works in normal browser but fails in:
```

## Reviewer checklist

Before marking a browser bug as “cannot reproduce,” ask:

- Is the exact path included?
- Do we know what action happened before the failure?
- Is there a first failure signal, not just the final screen?
- Is the before/after browser state clear?
- Are console/network/trace artifacts attached when relevant?
- Can another person rerun the report without a meeting?

## Related resources

- [Browser Bug Test Artifact Checklist](../browser-bug-test-artifact-checklist/)

## Built by Samelogic

Samelogic gives teams test artifacts for important browser work: the path, state, action, and first failure signal behind browser bugs.

- Website: https://samelogic.com
- Chrome Web Store: https://chromewebstore.google.com/detail/bmgbagkoginmbbgjapcacehjdojdnnhf
