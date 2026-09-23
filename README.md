# Shelf — builds and appcast

This repository holds only built downloads of [Shelf](https://github.com/Erikemmer/Shelf)
and the two feeds ([`appcast.xml`](appcast.xml) for stable releases,
[`appcast-beta.xml`](appcast-beta.xml) for release candidates) that its
in-app updater reads. No source code lives here — that stays in the main
repository, which is public itself.

## Installing

Download the `.zip` for the version you want from
[Releases](https://github.com/Erikemmer/shelf-releases/releases), unzip it,
and drag `Shelf.app` to `/Applications`.

**Until a Developer ID certificate exists, every build here is unsigned.**
Gatekeeper will say the app "cannot be opened because it is from an
unidentified developer" or that it "is damaged and should be moved to the
Trash" — the second message is misleading; it is what an unsigned app looks
like to a Mac that did not build it, not a sign of a broken download. To open
it anyway:

- Right-click (or Control-click) `Shelf.app` and choose **Open**, then
  confirm in the dialog that appears, **or**
- Go to **System Settings ▸ Privacy & Security**, scroll to the message
  about Shelf, and click **Open Anyway**.

This is a one-time step per version, not something you need to repeat every
launch.

## About updates

**Version 1.0.0 has no update mechanism at all.** If that is what you have,
downloading a newer version here is a manual, one-time step — the same as
above.

Starting with the version after it, Shelf checks for updates on its own
(never installing anything without asking first) and offers a manual
**Shelf ▸ Check for Updates…** as well. From then on, downloading here by
hand is only ever needed once — every update after that arrives through the
app itself.
