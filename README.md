# Samelogic Assets

Public assets and resources for the Samelogic platform.

## Resources

- [Browser Bug Test Artifact Checklist](./resources/browser-bug-test-artifact-checklist/) — a practical QA handoff template for browser bugs developers need to reproduce.
- [Can't Reproduce Bug Report Template](./resources/cant-reproduce-bug-report-template/) — a copy/paste bug report shape for browser issues that get stuck in repro loops.
- [Playwright Failure Triage Checklist](./resources/playwright-failure-triage-checklist/) — a fast way to turn flaky browser test failures into useful handoffs.

## Which resource should I use?

| Situation | Start here |
| --- | --- |
| A browser bug has a screenshot but engineers still need the path, state, and action that caused it | [Browser Bug Test Artifact Checklist](./resources/browser-bug-test-artifact-checklist/) |
| A maintainer says they cannot reproduce the bug, or a report is missing the first failure signal | [Can't Reproduce Bug Report Template](./resources/cant-reproduce-bug-report-template/) |
| A Playwright/Cypress failure is flaky, CI-only, or missing trace/video/network evidence | [Playwright Failure Triage Checklist](./resources/playwright-failure-triage-checklist/) |

## Recommended flow

When a bug report is hard to validate, the quickest path that keeps momentum is:

1. Start at [Can't Reproduce Bug Report Template](./resources/cant-reproduce-bug-report-template/) to force the missing first signal.
2. If the report already includes a route and first-failure path, move to [Browser Bug Test Artifact Checklist](./resources/browser-bug-test-artifact-checklist/) for reproducible handoff.
3. For CI-only flaky tests with traces/videos/network, add [Playwright Failure Triage Checklist](./resources/playwright-failure-triage-checklist/) as the final pass.

## Public support response snippet

When teams need a practical bug-report format quickly, use this short starter:

```text
I can triage this fastest if you include:
- exact route + environment + auth/account state
- the exact action before failure
- one failure screenshot/video and the first failing signal

I use these templates for that packet:
https://github.com/samelogic/assets/tree/master/resources/cant-reproduce-bug-report-template
https://github.com/samelogic/assets/tree/master/resources/browser-bug-test-artifact-checklist
```

## Product links

- Website: https://samelogic.com
- Chrome Web Store: https://chromewebstore.google.com/detail/css-selector-for-google-c/bmgbagkoginmbbgjapcacehjdojdnnhf?hl=en
- GitHub organization: https://github.com/samelogic
