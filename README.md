# Anyka-Micro `.github` repository

This is the special `.github` repository for the [Anyka-Micro](https://github.com/Anyka-Micro) organization. It's for **maintainers**. Visitors see the organization page, which is built from `profile/README.md`.

GitHub treats this repository specially. Some files here change what **every** repository in the organization shows, so treat edits with care.

## What each file does

| File | Importance | What GitHub does with it |
|---|---|---|
| `profile/README.md` | 🔴 **Critical**: public | The short landing page at github.com/Anyka-Micro: summary, Get started, warnings. Keep it minimal; the full list lives in [awesome-anyka](https://github.com/Anyka-Micro/awesome-anyka). |
| `profile/anyka-logo.png` | 🔴 **Critical**: public | The official logo at the top of the landing page. Replace it only with a file from Anyka's brand team. |
| `CONTRIBUTING.md` | 🔴 **Critical**: org-wide | The attribution policy. Also the default contributing guide for every org repo that doesn't have its own. |
| `.github/pull_request_template.md` | 🟠 **Important**: org-wide | The Must/Should checklist pre-filled into every new PR in every org repo without its own template. |
| `.github/ISSUE_TEMPLATE/*.yml` | 🟠 **Important**: org-wide | The *Suggest*, *Correct* and *Remove* forms, inherited by every org repo without its own. They apply the `project-suggestion`, `correction` and `removal-request` labels, which must exist in each repo that uses them. |
| `LICENSE` | ⚪ Reference | CC BY 4.0 for the text in this repository. The Anyka name and logo are excluded. |
| `README.md` (this file) | ⚪ Reference | Only shown when someone opens this repository. |
| `.gitignore` | ⚪ Housekeeping | Keeps local notes, research drafts and the local `awesome-anyka` checkout out of this repository. |

## Repositories in this organization

| Kind | Name | Example | Topic |
|---|---|---|---|
| Official SDK | `sdk-<chip>` | `sdk-ak3918ev300` | `anyka-sdk` |
| Official application | `app-<name>` | `app-ipcam-demo` | `anyka-app` |
| Index or documentation | no prefix | `awesome-anyka` | `awesome-list` |

Every repo also gets the `anyka` topic and a one-line description, because the org page shows both. Pin up to 6 repos (org page → **Customize pins**): `awesome-anyka` first, then official SDKs, then applications.

## Rules for this repository

- **`main` is protected** here and in `awesome-anyka`. Every change goes through a pull request with one approving review. While there is only one owner, the owner may merge with the admin bypass. Stop doing that once a second owner exists.
- **Listing changes go to [awesome-anyka](https://github.com/Anyka-Micro/awesome-anyka)** and follow [CONTRIBUTING.md](CONTRIBUTING.md). Read its "At a glance" section first: 🔴 Must rules block a merge, 🟡 Should rules don't.
- **Don't rename or move** `profile/README.md`, `.github/ISSUE_TEMPLATE/` or `.github/pull_request_template.md`. GitHub finds them by exact path, and moving them silently turns the feature off.

## Routine upkeep

| When | Task |
|---|---|
| Within 7 days of a `removal-request` issue | Remove the entry from awesome-anyka. No discussion needed. |
| On every `correction` issue | Fix the entry first, then discuss. |
| Every 6 months | Re-check the license and Status of every entry in awesome-anyka and update **Checked**. Review whether the profile's **Get started** picks are still the most used and active. |
| When Anyka publishes an official repo | Name it by the convention above, add it to awesome-anyka marked **Official**, and pin it. |

## Settings that live outside this repository

These are set by an org owner under the organization's **Settings**, not in files:

- **Profile:** display name, description, website, location and avatar (the square logo).
- **Verified & approved domains:** the company domain, which gives the org its **Verified** badge.
- **Code security:** private vulnerability reporting for all repositories.
- **Member privileges:** base permission **Read**.
- **People:** at least two owners. Membership stays private until the company account is set up.
