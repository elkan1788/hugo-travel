# Hugo Travel

## Overview

Learning Hugo Docs site used [Turbo](https://github.com/hotwired/turbo) implements SAP feature.

## Usage

Ready the Hugo binary than v0.146.0 and clone a speific branch starting test:

```bash
git clone --single-branch -b hugo-feature-turbo_sap https://github.com/elkan1788/hugo-travel hugo-feature-turbo_sap
cd hugo-feature-turbo_sap
hugo server
```

## Summary

There find that it very easy use Turbo implements SAP feature. If you not any script action, there only refer the script into your HTML code inside into  the `<head>` tag. And if you want make some action with user , then can through the Turbo's event into your JavaScript code.

> [!NOTE]
> Give up to used turbo-stream function, because it's need server output special template HTML code.

All Turbo Events sees as blew table shows:

| Event Name                  | Trigger Description                                  | Bubbles | Cancelable |
|-----------------------------|------------------------------------------------------|---------|------------|
| `turbo:click`               | Fired when an `<a>` link is clicked.                | ✅ Yes  | ❌ No      |
| `turbo:before-fetch-request`| Before a fetch request is made.                     | ✅ Yes  | ❌ No      |
| `turbo:before-fetch-response`| After response is received, before processing it.  | ✅ Yes  | ❌ No      |
| `turbo:before-cache`        | Before the page is cached.                          | ✅ Yes  | ❌ No      |
| `turbo:before-render`       | Before DOM is updated with new content.             | ✅ Yes  | ✅ Yes     |
| `turbo:render`              | After DOM has been updated.                         | ✅ Yes  | ❌ No      |
| `turbo:load`                | After initial page load or Turbo navigation ends.   | ✅ Yes  | ❌ No      |
| `turbo:frame-missing`       | When requested `<turbo-frame>` not found.           | ✅ Yes  | ❌ No      |
| `turbo:frame-render`        | When a `<turbo-frame>` is rendered.                 | ✅ Yes  | ✅ Yes     |
| `turbo:visit`               | When a new visit (navigation) begins.               | ✅ Yes  | ❌ No      |
| `turbo:before-visit`        | Before a visit is initiated.                        | ✅ Yes  | ✅ Yes     |
| `turbo:submit-start`        | When a form submission starts.                      | ✅ Yes  | ❌ No      |
| `turbo:submit-end`          | When a form submission completes.                   | ✅ Yes  | ❌ No      |
