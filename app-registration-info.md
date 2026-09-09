# TikTok Developer App Registration — Copy-Paste Fields

**App name:** Jarvis Income Assistant

**Category:** Content Management / Productivity (pick whichever category option
most closely matches "content publishing tool" in TikTok's dropdown)

**Description (shown to the account owner on the authorization screen):**
> Jarvis Income Assistant is a personal automation tool that generates and
> publishes short-form video content to a single TikTok account. It uploads
> finished videos on behalf of the account owner, who creates and reviews all
> content before it is authorized to publish.

**Website URL:** https://dannnne84.github.io/jarvis-income-assistant-site/

**Privacy Policy URL:** https://dannnne84.github.io/jarvis-income-assistant-site/privacy-policy.html

**Terms of Service URL:** https://dannnne84.github.io/jarvis-income-assistant-site/terms-of-service.html

**App icon:** site/app-icon.png (1024x1024, already generated)

**Scope to request:** `video.upload` (Content Posting API)

**Redirect URI:** needs a real endpoint that can receive TikTok's OAuth
callback and exchange the code for an access token — not yet built. Simplest
option once the app itself is approved: a small local script that runs a
one-time HTTP listener on localhost during setup (e.g. `http://localhost:8787/callback`),
since this only needs to run once per token refresh, not as a live server.

**Demo video for review:** not yet made — needs `post_to_tiktok.py` actually
running once we have test credentials, to record the real upload happening.
