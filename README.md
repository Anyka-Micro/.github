# Anyka-Micro `.github` repository

This is the special `.github` repository for the [Anyka-Micro](https://github.com/Anyka-Micro) organization. It's for **maintainers**. Visitors see the organization page, which is built from `profile/README.md`.

GitHub treats this repository specially. Some files here change what **every** repository in the organization shows, so treat edits with care.

## What each file does

| File | Importance | What GitHub does with it |
|---|---|---|
| `profile/README.md` | 🔴 **Critical**: public | Rendered as the organization's landing page at github.com/Anyka-Micro. Every change is immediately public. |
| `profile/anyka-logo.png` | 🔴 **Critical**: public | The official logo shown at the top of the landing page. Replace it only with a file from Anyka's brand team. |
| `CONTRIBUTING.md` | 🔴 **Critical**: org-wide | The attribution policy. Also used as the default contributing guide for every org repo that doesn't have its own. |
| `.github/pull_request_template.md` | 🟠 **Important**: org-wide | The checklist pre-filled into every new PR, here and in every org repo that doesn't have its own template. |
| `.github/ISSUE_TEMPLATE/*.yml` | 🟠 **Important**: org-wide | The *Suggest*, *Correct* and *Remove* forms. They apply the `project-suggestion`, `correction` and `removal-request` labels. Default forms for org repos without their own. |
| `README.md` (this file) | ⚪ Reference | Only shown when someone opens this repository. It doesn't appear on the org page. |
| `.gitignore` | ⚪ Housekeeping | Keeps local working notes and research drafts out of the repository. |

## Rules for this repository

- **`main` is protected.** Every change goes through a pull request with one approving review. While there is only one owner, the owner may merge with the admin bypass. Remove that habit once a second owner exists.
- **Profile edits follow [CONTRIBUTING.md](CONTRIBUTING.md).** Read its "At a glance" section first: the 🔴 Must rules block a merge, the 🟡 Should rules don't.
- **Don't rename or move** `profile/README.md`, `.github/ISSUE_TEMPLATE/` or `.github/pull_request_template.md`. GitHub finds them by exact path, and moving them silently turns the feature off.
- **Keep the labels.** The issue forms rely on `project-suggestion`, `correction` and `removal-request` existing.

## Routine upkeep

| When | Task |
|---|---|
| Within 7 days of a `removal-request` issue | Remove the entry. No discussion needed. |
| On every `correction` issue | Fix the entry first, then discuss. |
| Every 6 months | Re-check the license and Status of every listed project and update **Checked**. Review whether the **Start here** picks are still the most used and active. |
| When Anyka publishes an official repo | Add it to the profile marked **Official**, and update the "Get official Anyka SDKs" row in **Start here**. |

## Settings that live outside this repository

These are set by an org owner under the organization's **Settings**, not in files:

- **Profile:** display name, description, URL and avatar (the square logo).
- **Verified & approved domains:** the company domain, which gives the org its **Verified** badge.
- **Member privileges:** base permission **Read**.
- **People:** at least two owners, and membership visibility.
