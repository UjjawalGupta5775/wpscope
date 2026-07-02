# WPScope — Privacy Policy

**Last updated: 2 July 2026**

WPScope is a Chrome extension that inspects WordPress websites **locally in your browser**.
This policy explains what it does and does not do with data.

## Data we collect

**None.** WPScope does not collect, store on any server, or transmit your personal data.
We operate no servers, no accounts, and no analytics or tracking of any kind.

## Local storage

Your settings, saved REST API endpoints, request history, per-site notes, and cached audit
results are stored **locally in your browser** using the standard `chrome.storage` API. This
data stays on your device and is never sent to us or any third party, except for the optional
lookups described below.

## Optional network lookups (off by default)

WPScope works entirely offline for its core inspection. If — and only if — you explicitly
enable **"directory lookups"** or **"threat lookups"** in the extension's Settings, WPScope
contacts public third-party APIs to enrich results:

- **api.wordpress.org** — public plugin/theme names, versions, and install counts (sends only a
  public plugin/theme slug).
- **WPVulnerability / URLhaus** — public known-vulnerability and malicious-domain advisory data.
- **The inspected site's own public endpoints** — e.g. `/wp-json/`, `robots.txt`, `sitemap.xml`
  of the site you choose to inspect.

These requests contain only **public identifiers** (plugin slugs, and the URL of the site you
are actively inspecting). **No personal data is transmitted.** You can turn these lookups off at
any time in Settings, and they are off until you turn them on.

## Permissions

WPScope requests broad host access so it can inspect **any** WordPress site you choose to open —
a WordPress site can live on any domain, so a fixed list is not possible. Using this access,
WPScope reads the content of the page you are inspecting and makes **read-only** requests to that
same site. It does **not** modify websites, does **not** perform intrusive or attack-style
testing, and collects **no** data. It is a passive, browser-side developer tool intended for
sites you own or are authorized to work on.

## Children's privacy

WPScope is a developer tool and is not directed at children. It collects no personal data from
anyone.

## Changes to this policy

If this policy changes, the "Last updated" date above will change. Material changes will be
reflected here before they take effect.

## Contact

Questions about this policy? Open an issue at the project's GitHub repository:
**https://github.com/UjjawalGupta5775/wpscope/issues**
