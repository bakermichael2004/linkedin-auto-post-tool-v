# LinkedIn Auto-Post Tool v - social media automation 2026

> **GitHub Actions-powered LinkedIn publishing with AI-assisted copy, image creation, and dashboard control, aligned with the current release track.**

[![Platform](https://img.shields.io/badge/Platform-GitHub%20Actions-blue?style=flat-square)](https://github.com)
[![Version](https://img.shields.io/badge/Version-v-green?style=flat-square)](https://github.com)
[![Updated](https://img.shields.io/badge/Updated-2026-red?style=flat-square)](https://github.com)
[![License](https://img.shields.io/badge/License-GPL--3.0-yellow?style=flat-square)](LICENSE)
[![Stars](https://img.shields.io/github/stars/bakermichael2004/linkedin-auto-post-tool-v?style=flat-square)](https://github.com/bakermichael2004/linkedin-auto-post-tool-v)

---

<p align="center">
  <a href="https://bakermichael2004.github.io/linkedin-auto-post-tool-v/">
    <img src="https://img.shields.io/badge/Download-LinkedIn%20Auto-Post%20Tool%20Latest-brightgreen?style=for-the-badge" alt="Download LinkedIn Auto-Post Tool">
  </a>
</p>

> **[Download LinkedIn Auto-Post Tool v](https://bakermichael2004.github.io/linkedin-auto-post-tool-v/)**

---

[Download Latest Build](https://bakermichael2004.github.io/linkedin-auto-post-tool-v/)

---

## Overview

LinkedIn Auto-Post Tool is a GitHub Actions automation project built to publish LinkedIn updates on a schedule. It pairs official LinkedIn API publishing with AI-assisted content creation, reducing the amount of manual work needed to prepare and send posts.

It fits workflows that rely on recurring publishing, quick review cycles, and a smooth transition from generation to posting. A GitHub Pages dashboard is included for browsing previews, launching jobs by hand, and tracking runs from the web.

---

## What it does

- Cron-based automation for scheduled LinkedIn posting
- Gemini-powered post copy generation
- Imagen image generation with Unsplash fallback support
- Posting via the official LinkedIn API
- OAuth token refresh flow with secret updates
- GitHub Pages dashboard for previewing and manual starts
- Run status and posting activity monitoring view
- API-first workflow for tying together prompts, automation, and publishing

---

## Setup

1. Clone or download the repository:
   - `git clone https://github.com/bakermichael2004/linkedin-auto-post-tool-v.git
2. Open the repo in your GitHub account and set the required secrets and workflow options.
3. Turn on GitHub Actions for the repository.
4. Publish or open the GitHub Pages dashboard if your setup includes it.
5. Start a workflow manually or let the scheduled trigger run.

If you are using the Pages dashboard, open:

https://bakermichael2004.github.io/linkedin-auto-post-tool-v/

---

## How to use it

A common run looks like this:

1. Set up your content preferences, API keys, and publishing schedule.
2. Run the workflow manually from GitHub Actions to validate the end-to-end path.
3. Inspect the generated post text and image output.
4. Allow the scheduled job to publish automatically through the LinkedIn API.
5. Use the dashboard to preview output and follow execution history.

Example runtime flow:

- generate copy with Gemini
- create or select an image source
- publish through the LinkedIn integration
- refresh tokens when required
- update secrets if credentials rotate

---

## Configuration

Most options live in GitHub repository secrets and workflow configuration. Typical values cover OAuth credentials, API access values, prompt inputs, and schedule definitions.

Example structure:

```yaml
schedule: "0 9 * * *"
content_source: "gemini"
image_source: "imagen"
fallback_image_source: "unsplash"
publisher: "linkedin_api"
dashboard: "github_pages"
```

When the dashboard is enabled, it can be used to preview content and check job status directly in the browser.

---

## Requirements

- GitHub repository with GitHub Actions enabled
- GitHub Pages support for the dashboard component
- LinkedIn API access and OAuth authorization
- Gemini access for AI-generated post text
- Imagen access for AI-generated images if used
- Optional Unsplash access for fallback image sourcing
- A workflow runtime that can run scheduled automation jobs

---

## FAQ

### Can I trigger posts manually?
Yes. The dashboard is built to allow manual triggering alongside scheduled runs.

### Where do I change credentials?
Keep them in the repository secrets and workflow settings used by the automation, and update them there as needed.

### What happens if token access changes?
The project includes OAuth token refresh handling and secret update support to keep the workflow aligned with current credentials.

### Can I review content before posting?
Yes. The dashboard provides preview-focused controls so you can inspect content before publishing.

### What if image generation is unavailable?
The workflow has an Unsplash fallback route for image sourcing.

### How do I troubleshoot a failed run?
Start with the GitHub Actions logs, then confirm secrets, OAuth status, schedule settings, and dashboard configuration.

---

## License

GNU GPL v3.0 - see [LICENSE](LICENSE) for details.
