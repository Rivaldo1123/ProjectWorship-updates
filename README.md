# Project Worship — Updates

Public **binary-only update feed** for [Project Worship](https://github.com/Rivaldo1123/ProjectWorship),
a Windows desktop worship-projection app by **Valdo Enterprises**.

This repository exists so the app's in-app Update Center (GitHub Releases channel)
has a public place to fetch installers and update metadata **without exposing the
private application source**. GitHub auto-generates a source archive for every
tagged release; by publishing releases here — a repository that contains no source —
those archives stay small and public-safe.

## What belongs here

Published only as **GitHub Release assets** (not committed to the default branch):

- Windows installer files (`Project Worship-<version>-setup.exe`)
- Update metadata (`latest.yml`)
- Blockmap / differential-update files (`*.exe.blockmap`)
- Release notes / version information

## What must NEVER be here

- App **source code**
- Private product documentation, specs, or internal design docs
- Credentials, tokens, or signing secrets
- Church workspaces, databases, backups, logs, or test data
- Unreviewed or development builds

## How releases get here

Releases are built from the **private** `ProjectWorship` source repository and
published here (electron-builder is configured with
`publish.repo: ProjectWorship-updates`). Development and CI never publish from the
private source repo. As of this writing the app's Update Center is **prepared but
not yet connected** — no release has been published; this repository is the
provisioned, empty destination for the first one.

---

Maintained by **Valdo Enterprises**.
