# Burger Boat Company - public files

Files that Burger Boat Company publishes for anyone to read, such as brand images that
company PCs download before anyone signs in.

**Everything here is public.** Never add anything that isn't meant for anyone to see:
no internal documents, configuration, names, addresses, credentials or tokens.

## Contents

| Path | What it is | Used by |
|---|---|---|
| `windows/lock-screen/` | Windows lock screen pictures | Intune policies `BBC-Lock Screen Image*` |

The source, build steps and SHA-256 of each lock screen picture are kept in Burger Boat's
private IT repository under `ops/m365/lock-screen/`.

## Rules

- **Never replace, rename or delete a published file while something points at it.** Windows
  caches the lock screen picture, so new bytes at the same address may never reach the PCs.
  A new picture gets a new, dated file name.
- Changes reach `main` only through a reviewed pull request.
