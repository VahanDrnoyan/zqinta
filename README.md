# zQinta — Public Support Repo

Public-facing support site for **zQinta** (a macOS app). Kept separate from the private source repository so that:

- 🔒 The app source stays **private**.
- 🌐 End users can **open GitHub Issues** here (impossible on a private repo).
- 🆓 **GitHub Pages** hosts the Support and Privacy Policy pages for free — the two URLs Apple requires in App Store Connect.

---

## What's in here

| File | Purpose | App Store Connect field |
|---|---|---|
| `support.md` | Support page (how to get help, report bugs, refunds) | **Support URL** |
| `privacy.md` | Privacy policy | **Privacy Policy URL** |
| `.github/ISSUE_TEMPLATE/bug_report.md` | Pre-fills new issues with the info you need to triage | — |

---

## Publish via GitHub Pages (free, ~1 min)

1. Repo → **Settings → Pages**.
2. **Source:** `Deploy from a branch`.
3. **Branch:** `main` / `(root)` → **Save**.
4. Wait ~1 min. Site goes live.

Then paste these into **App Store Connect → App Information**:

- **Support URL:** `https://vahandrnoyan.github.io/zqinta/support.html`
- **Privacy Policy URL:** `https://vahandrnoyan.github.io/zqinta/privacy.html`
- **Issues:** `https://github.com/VahanDrnoyan/zqinta/issues`

> **Note on URLs:** GitHub Pages renders `support.md` to `/support.html` (Jekyll is on by default). The raw `/support.md` link also works but the rendered `.html` page looks cleaner for the App Store.

---

## When to update

- New known issues → edit the **Known issues** section in `support.md`.
- Privacy-relevant changes (new data flows, new AI providers, sync changes) → update `privacy.md` and bump the "Last updated" date.
- New app version with user-facing changes → optional note on the support page.
