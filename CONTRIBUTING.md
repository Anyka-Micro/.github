# Contributing & Attribution Policy

This is Anyka's official GitHub organization. Its repositories are Anyka's own, but most of the projects listed in [awesome-anyka](https://github.com/Anyka-Micro/awesome-anyka) are **community work**, published on their authors' own accounts under their own terms. Our job is to point to that work accurately, credit it properly, and never take more than its license allows. Because we are the vendor, we hold ourselves to a higher standard than a community index would.

Every maintainer follows these rules. Rules 1–4 and 7 apply to community projects. Rules 5, 6 and 8 cover how official and community work fit together. The PR checklist (`.github/pull_request_template.md`) enforces them.

## At a glance

### 🔴 Must: a PR that breaks any of these doesn't get merged

| Rule | Why it matters |
|---|---|
| Link the **upstream** repo. Never re-host community code. | Re-hosting without permission is copyright infringement, and coming from the vendor it's especially damaging. (§1) |
| Credit the author by GitHub handle. | It's their work. (§2) |
| Write descriptions in your own words. | Copying READMEs or images can infringe copyright. (§3) |
| Copy the license **exactly**, and mark unlicensed repos `No license — link only`. | Users decide what they may legally do based on this column. (§4) |
| Don't list third-party copies of Anyka SDKs, BSPs or datasheets. | Only Anyka decides what of its IP is released. (§5) |
| Mark entries **Official** or **Community** correctly. | Official means Anyka supports it. A wrong label is a support and legal promise. (§6) |
| Honor removal requests within 7 days. | Authors control whether they're associated with a vendor. (§7) |
| Fill every column, including **Status** and **Checked**. | An entry without them can't be trusted. |

### 🟡 Should: good practice, but not a merge blocker

- Notify the author after listing their project. (§7)
- Ask authors of unlicensed repos to add a license. (§4)
- Re-check the license and Status of every entry at least every 6 months, and update **Checked**.
- Add `CITATION.cff` to official repos that people may cite. (§8)

### What we list, and what we don't

| ✅ List | ❌ Don't list |
|---|---|
| SDKs, toolchains and build tooling | Third-party copies of Anyka SDKs, BSPs, datasheets or firmware dumps (§5) |
| Open firmware and applications with real code | Exploits, vulnerability write-ups, or tools that bypass a manufacturer's cloud or security checks. Report vulnerabilities privately instead. |
| Projects with a license, or clearly marked `No license — link only` | Repos that bundle Anyka binaries, unless the release owner has approved them (§5) |
| Projects pushed in the last 12 months, or older ones that are still the reference others build on | Empty, placeholder or dead-link repos |

The **Get started** list on the profile picks entries by usage (stars, forks, how many projects build on them) and recent activity. Keep it to one pick per goal, and never mark a project "recommended": Anyka doesn't endorse Community projects.

---

## 1. Link, don't copy

- Link to the **upstream repository**, not to a copy of it.
- Do **not** re-upload, mirror, or vendor someone else's code, binaries, or docs into this organization unless their license allows it **and** every copyright notice and license file is kept.
- To build on a project, use GitHub's **Fork** button (never download-and-re-push). A real fork keeps the upstream link and contributor history visible in GitHub's network graph.
- The first line of a fork's README must say: `Fork of [owner/repo](https://github.com/owner/repo) by @owner.`

## 2. Credit the author by name

- Every entry shows the author's GitHub handle, linked to their profile.
- For forks, credit **both**: the original author and the fork maintainer.
- If a project builds heavily on another (for example, a reverse-engineering write-up), name the upstream in the description too.

## 3. Use your own words

- Write each description yourself, in one or two sentences.
- Short quotes are fine: at most one sentence, inside quotation marks, with a link back to the source.
- Do not copy README sections, screenshots, logos, or diagrams. Use an image only if its license allows reuse or the author agreed, and credit it right next to the image.

## 4. Report the license exactly as upstream states it

- Use the SPDX identifier from the repo's `LICENSE` file, as shown in GitHub's "About" sidebar (for example `GPL-2.0`, `MIT`, `Apache-2.0`).
- **No LICENSE file means all rights reserved.** List it as `No license — link only`. Never fork-and-redistribute it. You can open a polite issue asking the author to add a license.
- Never guess or "upgrade" a license. If it's unclear, write `Unclear — see repo`.
- Record the **date you checked** (`Checked` field), because licenses can change.

## 5. Third-party copies of Anyka SDKs, BSPs, and datasheets

Many "Anyka SDK" repositories on GitHub are Anyka BSP releases or datasheets that third parties uploaded.

- **Don't list them** in awesome-anyka. Where an official release exists, link to that instead.
- Report each one to the release owner at Anyka (ask an org owner if you don't know who that is). Any takedown or licensing decision is the company's to make, not an individual maintainer's.
- Before publishing anything official, the release owner confirms what can be released. GPL components (Linux kernel, U-Boot, BusyBox) must ship with their corresponding source. Proprietary libraries and blobs need a stated license.
- **Never publish internal or confidential material** (unreleased SDKs, NDA datasheets) in this organization without written release approval.

## 6. Official vs community: keep the line clear

- Mark a repo **Official** only if it lives in this organization and Anyka maintains it.
- Mark everything else **Community**. Listing a community project doesn't mean Anyka supports it, and doesn't mean its author is affiliated with Anyka.
- Never suggest that a community author works for or speaks for Anyka.
- Anyka's logo and name are ours to use. Don't put them on a community project's entry in a way that makes it look like an Anyka product.

## 7. Be a good neighbour

- After listing a project, tell the author. A short issue or discussion post on their repo is enough: *"We've linked your project from https://github.com/Anyka-Micro. Happy to update or remove the entry on request."*
- **Removal requests:** if an author asks to be unlisted (by an issue labelled `removal-request` here, or by any other channel), remove the entry within 7 days. No debate.
- **Corrections** (wrong license, wrong author, wrong chip support) get fixed first and discussed afterwards.

## 8. Our own repositories

Repos created in this organization must include:

- `LICENSE` (an OSI-approved license)
- a **Credits** section in the README naming every upstream project they build on
- `CITATION.cff`, if people may cite the work academically (GitHub then shows "Cite this repository")
- the original copyright and license headers on any third-party file they contain

---

## Adding a project to awesome-anyka

1. Choose the section:
   - **SDKs & low-level tooling:** toolchains, BSPs, kernel/U-Boot trees, flashing and recovery tools, register docs.
   - **Applications:** firmware images, camera and streaming apps, integrations built on the SDKs.
2. Copy the **Official** or **Community** row template from the comment in [awesome-anyka's README](https://github.com/Anyka-Micro/awesome-anyka) and add the row to that section's table.
3. Fill in **every** column. A row with an empty column doesn't get merged. Set **Status** from the repo's last push: 🟢 Active within the last 12 months, ⚪ Inactive (with the month of the last push) if older, 📦 Archived if the owner archived it.
4. Open a PR and complete the checklist. Another admin must approve it before merging.
