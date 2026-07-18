# Browser Bug Test Artifact Checklist

## Create test artifacts with the Samelogic Chrome extension

You can create the test artifacts described in this guide directly from your browser. The Samelogic Chrome extension makes it easy to capture and share replayable proof of the path, page state, element, action, and first failure signal behind a browser bug.

- [Install the Samelogic Chrome extension](https://chromewebstore.google.com/detail/css-selector-for-google-c/bmgbagkoginmbbgjapcacehjdojdnnhf?hl=en)
- [Learn more about Samelogic](https://samelogic.com)
- [Visit Samelogic on GitHub](https://github.com/samelogic)

A screenshot shows where the bug ended. A test artifact shows what happened.

This is a Samelogic public resource for QA, support, product, and engineering teams that need browser bug reports developers can actually trust.

## Download

- [Markdown checklist](./browser-bug-test-artifact-checklist.md)

## Why this exists

Most browser bug reports fail during handoff because they capture the final broken screen but not the path, state, action, delta, and first failure signal that got the user there.

Use this checklist when a bug report, support escalation, QA artifact, or browser automation failure needs to be inspectable without another screenshare.

## One-line rule

If engineering has to ask “what happened before the screenshot?”, the report is missing the test artifact.

## Related resources

- [Can't Reproduce Bug Report Template](../cant-reproduce-bug-report-template/)
- [Playwright Failure Triage Checklist](../playwright-failure-triage-checklist/)

## Use this in public replies

Use the GitHub folder URL when someone asks for a practical QA bug-report checklist or a better way to describe “cannot reproduce” browser bugs:

```text
A screenshot shows where the bug ended. A test artifact shows what happened.

We keep a practical checklist here:
https://github.com/samelogic/assets/tree/master/resources/browser-bug-test-artifact-checklist
```
