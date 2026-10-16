# Anyka Open Source

The official GitHub home for open-source SDKs, tools and applications for the **Anyka SoC family** (AK3918 and others).

Much of the open-source work for these chips has been done by the community, on community members' own accounts. We list it here together with Anyka's own releases and credit every author. Each entry is marked **Official** (maintained by Anyka) or **Community** (maintained by its author). **Every project keeps its own license.** Before you use, fork or redistribute a project, check the license in its repository.

---

## 🧰 SDKs & low-level tooling

Toolchains, BSPs, kernel and U-Boot trees, flashing and recovery tools.

| Project | Maintainer | What it is | Chips | License | Checked |
|---|---|---|---|---|---|
| [OpenIPC/firmware](https://github.com/OpenIPC/firmware) | Community · [@OpenIPC](https://github.com/OpenIPC) | Buildroot-based replacement firmware for IP cameras from many SoC vendors; its Anyka layer has board configs for the AK3916EV300 and AK3918EV300. | AK3916EV300, AK3918EV300 | MIT | 2026-10-16 |
| [Nemobi/arm-anykav200-crosstool-docker](https://github.com/Nemobi/arm-anykav200-crosstool-docker) | Community · [@Nemobi](https://github.com/Nemobi) | A Dockerfile that packages the anykav200 cross toolchain into a container image. | AK3918 (anykav200 toolchain) | No license — link only | 2026-10-16 |
| [MXDMY/ak37e_lvgl8](https://github.com/MXDMY/ak37e_lvgl8) | Community · [@MXDMY](https://github.com/MXDMY) | A port of the LVGL 8.2 graphics library to the AK37E platform, meant as a starting template for GUI apps. The repo is archived. | AK37E | Apache-2.0 | 2026-10-16 |

## 📷 Applications

Firmware, camera and streaming apps, and integrations built on the SDKs above.

| Project | Maintainer | What it is | Chips | License | Checked |
|---|---|---|---|---|---|
| [MuhammedKalkan/Anyka-Camera-Firmware](https://github.com/MuhammedKalkan/Anyka-Camera-Firmware) | Community · [@MuhammedKalkan](https://github.com/MuhammedKalkan) | SD-card based custom firmware and apps (RTSP, web UI, PTZ) for AK3918 cameras. Many later projects build on it. | AK3918 (tested on AK3918v200EN080) | MIT | 2026-10-16 |
| [kkrzysztofik/Anyka_ak3918_hacking_journey](https://github.com/kkrzysztofik/Anyka_ak3918_hacking_journey) | Community · [@kkrzysztofik](https://github.com/kkrzysztofik) | An actively maintained continuation of Gerge's AK3918 hacking project (originally on Gitea), adding fixes and a Rust rewrite of the ONVIF services. | AK3918 | GPL-3.0 | 2026-10-16 |
| [ThatUsernameAlreadyExist/anyka-v4l2rtspserver](https://github.com/ThatUsernameAlreadyExist/anyka-v4l2rtspserver) | Community · [@ThatUsernameAlreadyExist](https://github.com/ThatUsernameAlreadyExist) | An AK3918 port of mpromonet's v4l2rtspserver RTSP server. | AK3918 | Unlicense | 2026-10-16 |
| [dangerousplay/kamoder](https://github.com/dangerousplay/kamoder) | Community · [@dangerousplay](https://github.com/dangerousplay) | Replacement camera firmware written in Rust that boots from the SD card, with RTSP, ONVIF, PTZ and a web UI. | AK3918 (EV200, AV100) | GPL-3.0 | 2026-10-16 |
| [michelostojski/akost-firmware](https://github.com/michelostojski/akost-firmware) | Community · [@michelostojski](https://github.com/michelostojski) | A Buildroot external tree that builds open firmware for AK39EV330 cameras such as the GNCC GK2, with RTSP and ONVIF. | AK39EV330 | MIT | 2026-10-16 |
| [jphein/anyka3918-gc1084-camera](https://github.com/jphein/anyka3918-gc1084-camera) | Community · [@jphein](https://github.com/jphein) | Local RTSP, PTZ and Home Assistant support for AK3918 cameras with a GC1084 sensor, such as the Teruhal TC20. | AK3918 | GPL-3.0 | 2026-10-16 |
| [SotosSW/anykav380-ak3918-hacking](https://github.com/SotosSW/anykav380-ak3918-hacking) | Community · [@SotosSW](https://github.com/SotosSW) | Takes V380-style AK3918 cameras off the cloud with RTSP, ONVIF and an improved PTZ daemon. Builds on work by MuhammedKalkan and kuhnchris. | AK3918 | GPL-3.0 | 2026-10-16 |

<!--
  ROW TEMPLATE. Every column is required (see CONTRIBUTING.md).
  Official:  | [Anyka-Micro/REPO](https://github.com/Anyka-Micro/REPO) | **Official** · Anyka | One sentence. | AK3918EV300 | SPDX-ID | YYYY-MM-DD |
  Community: | [OWNER/REPO](https://github.com/OWNER/REPO) | Community · [@OWNER](https://github.com/OWNER) [, fork of [x/y](…)] | One sentence, your own words. | AK3918EV300 | SPDX-ID / No license — link only / Unclear — see repo | YYYY-MM-DD |
-->

---

## Add, correct or remove a project

- **Suggest a project:** open an issue in the [`.github` repo](https://github.com/Anyka-Micro/.github/issues/new) with a link to it.
- **Community author and want to be unlisted?** Open an issue labelled `removal-request`. We'll remove the entry within 7 days, no questions asked.
- **Something wrong?** We fix corrections to licenses, authors or chip support first.
- **Maintainers:** read the [contribution & attribution policy](https://github.com/Anyka-Micro/.github/blob/main/CONTRIBUTING.md) before adding entries.

---

<sub>Projects marked **Community** are the work of their respective authors and are listed for convenience. Anyka does not maintain, support or warrant them, and listing a project doesn't mean its author is affiliated with Anyka. Flashing custom or community firmware can permanently damage your device and may void your warranty. Proceed at your own risk.</sub>
