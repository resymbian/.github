<p align="center">
  <img src="https://hosted.inled.es/cdn/resymbian-logo-symbian-horizontal.png" alt="Resymbian" width="420">
</p>

# Resymbian

**Keeping Symbian usable today.** Clients, bridges and build tooling for the
phones people still carry, written so that anyone can rebuild them and check
what they run.

This is my personal work and, just as much, my learning process. Nobody pays for
it; I write it because I want more people to be able to use Symbian today with
the comfort and safety of a current device: a chat client that still works, a
notification that actually arrives, a build you can reproduce instead of a
binary someone uploaded once.

## What that means in practice

- **Reproducible builds.** Every artefact comes from a workflow you can read and
  rerun, with pinned toolchains and checksums, from source in the repository.
  Where a proprietary SDK is unavoidable, the recipe is public and the download
  is pinned by SHA-256.
- **Comfort.** The clients are meant to be used daily on a keypad phone: small
  memory footprint, background notifications, attachments, settings that
  survive a reboot.
- **Safety.** No proxies that see your session, no third-party servers in the
  middle, no unverifiable binaries. TLS, signing and release provenance are
  part of the work, not an afterthought.
- **Clients for what is actually required today.** The services people use are
  not going to make a J2ME build for them, so the clients exist here: Discord,
  Telegram, and the native pieces those clients need to behave like modern apps
  on a 2007 handset.

## Projects

| Project | What it is |
| --- | --- |
| [Discofi](https://github.com/resymbian/Discofi) | Discord client for J2ME phones (MIDP 2.0 / CLDC 1.0), forked from gtrxAC's client and extended for daily use on the Nokia E51. |
| [ResyGram](https://github.com/resymbian/ResyGram) | Telegram client for MIDP 2.0 / CLDC 1.1 phones, with attachments, file uploads and background notifications. |
| [NotiHelper](https://github.com/resymbian/NotiHelper) | Native S60 3rd bridge: loopback socket in, system note and Messaging Inbox entry out. Built and signed in GitHub Actions. |
| [for-devs](https://github.com/resymbian/for-devs) | Tooling and notes for developing for Symbian without a museum of old PCs. |
| [Kutegram](https://github.com/resymbian/Kutegram) | sisGram, an unofficial Telegram client for Symbian^3 / Belle, forked from Kutegram. |

## Status, honestly

These are working projects, not polished products. Not everything has been
tested on every handset, and the repositories say where that is the case:
limitations are documented next to the feature, not hidden in a roadmap. If a
platform makes something impossible, the README explains why instead of
promising it.

If you have an old phone in a drawer, that is the target audience.
