# wyper browser extensions

Two free browser extensions for Chrome, Brave and Firefox, made by [wyper.io](https://wyper.io).

| Extension | What it does | Install |
|---|---|---|
| **wyper Social Cleanup** | Bulk delete tweets, likes and replies on X, bulk delete Instagram posts, comments, likes and DMs, bulk delete ChatGPT conversations. No OAuth, no password: runs in the tab you are already logged into. | [Chrome Web Store](https://chromewebstore.google.com/detail/aaekmgblkicfafjchfplgeadcbfddcea) · [Firefox Add-ons](https://addons.mozilla.org/firefox/addon/wyper-delete-tweets-posts/) |
| **wyper Fact-Check** | Fact-check a claim, article, image or video with real sources: a 1 to 10 truth score, the sources for and against, and the reasoning. | [Chrome Web Store](https://chromewebstore.google.com/detail/cfmfghjlfoilambbajgacdngkpfgjjkb) · [Firefox Add-ons](https://addons.mozilla.org/firefox/addon/wyper-ai-fact-check/) |

Current versions: Social Cleanup 1.6.46, Fact-Check 1.9.5 (both stores, November 2026).

This repository holds the public documentation, changelog and issue tracker for both extensions. The shipped packages are plain, unminified JavaScript: what you install is what you can read in the store package.

## wyper Social Cleanup

**Platforms:** X (Twitter), Instagram, ChatGPT.

**Actions**
- X: delete posts, replies, reposts, likes
- Instagram: delete posts, comments, likes; unsend direct messages; remove followers; unfollow
- ChatGPT: delete conversations by count, pinned chats are skipped
- Keyword filter on X posts and replies, with an invert option (delete everything except what matches)
- Live counter, safe speed by default, slow mode for the riskiest actions
- Optional counts-only cleanup receipt you can publish

**Free and Pro:** 50 removals a day free, any age, all filters. Pro: unlimited removals.

**What it does not do:** no date-range filter, no engagement filter, no export or backup, no archive import, no scheduling. Comparisons with tools that have these: [TweetDelete alternative](https://wyper.io/tweetdelete-alternative), [Redact alternative](https://wyper.io/redact-alternative), [wyper vs DeleteTweets](https://wyper.io/wyper-vs-deletetweets), [wyper vs DeclutterGPT](https://wyper.io/wyper-vs-decluttergpt).

**Privacy:** deletion runs inside your own browser session. No password, no OAuth grant, no token leaves the browser. The extension contacts `api.wyper.io` only to validate a licence key and, only when you choose to publish a receipt, to anchor that receipt (counts and a hash, never content). Bulk actions automate your own session, which is against the terms of service of X, Instagram and OpenAI; accounts can be rate-limited. Deletion is permanent.

Guides: [mass delete tweets](https://wyper.io/how-to-mass-delete-tweets.html) · [bulk delete Instagram posts](https://wyper.io/how-to-bulk-delete-instagram-posts.html) · [delete Instagram DMs](https://wyper.io/instagram-delete-dms) · [ChatGPT bulk delete](https://wyper.io/chatgpt-bulk-delete)

## wyper Fact-Check

- Highlight any text, right-click "Fact-check with wyper", or paste an X post, YouTube link or article URL into the popup
- Videos are checked from their captions; a video without captions is analysed directly, labelled as AI video analysis
- Images: checks whether a picture shows what the post claims
- Every verdict carries linkable sources; an unsupported claim is shown as unverified, not as half true
- X Community Notes are shown next to the result when a post carries one
- Pro: two independent AI models (Google Gemini and xAI Grok) cross-check each claim, Full Spectrum reports with counter-views, private Proof Library

**Privacy:** checks run only when you ask. The text you submit is sent to wyper's server for verification; emails, phone numbers and card numbers are stripped locally first. No browsing history, no tracking profile. AI fact-checkers can be wrong: open the sources.

Guides: [how to fact-check a claim or video](https://wyper.io/how-to-fact-check-a-video-or-claim.html) · [fact-checking tools compared](https://wyper.io/fact-checking-tools-compared) · [verify war footage](https://wyper.io/verify-war-footage)

## Changelog

See [CHANGELOG.md](CHANGELOG.md).

## Issues and support

Open an issue here or write to support@wyper.io. Privacy policy: https://wyper.io/privacy.html · Terms: https://wyper.io/terms.html
