# Playwright Failure Triage Checklist

Use this when a Playwright, Cypress, or browser E2E failure needs to become a clean handoff instead of another vague flaky-test thread.

Best fit: CI-only failures, WebKit/browser-specific flakes, timeout loops, missing trace/video evidence, and test failures where the final assertion is visible but the first failure signal is not.

## Triage fields

1. **Spec + step**
   - test file
   - test title
   - failing step or assertion
   - retry count

2. **Action attempted**
   - click/type/navigation/assertion
   - locator used
   - target element visible/enabled/stable?

3. **Settlement evidence**
   - did navigation finish?
   - did the expected request complete?
   - did the DOM/text/value change?
   - did the URL change?

4. **First failure signal**
   - timeout
   - detached element
   - strict mode violation
   - hidden/covered element
   - network/API failure
   - assertion mismatch
   - browser crash

5. **Artifacts**
   - trace zip
   - screenshot
   - video
   - console errors
   - network log/HAR
   - CI run URL

6. **Repro shape**
   - local only / CI only
   - headed / headless
   - browser + version
   - dataset/user/account state
   - pass/fail on retry

## Useful summary format

```text
Failure:
[short description]

First failure signal:
[earliest divergence]

Locator/action:
[locator + action]

Expected settlement:
[what should have changed]

Observed settlement:
[what changed or did not change]

Artifacts:
[trace/video/screenshot/logs]

Repro pattern:
[local/CI/browser/retry behavior]
```

## Related resources

- [Browser Bug Test Artifact Checklist](../browser-bug-test-artifact-checklist/)
- [Can't Reproduce Bug Report Template](../cant-reproduce-bug-report-template/)

## Built by Samelogic

Samelogic gives teams test artifacts for important browser work: the path, state, action, and first failure signal behind browser bugs.

- Website: https://samelogic.com
- Chrome Web Store: https://chromewebstore.google.com/detail/bmgbagkoginmbbgjapcacehjdojdnnhf
