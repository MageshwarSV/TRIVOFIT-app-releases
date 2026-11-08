# TRIVOFIT KERNEL — Android releases

Built APKs for the TRIVOFIT KERNEL app, the vendor-side control room for
TRIVOFIT. **No source code lives here** — this repository is public only so
that installed copies of the app can check for updates without credentials.

## Installing

Download the newest `.apk` from [Releases](../../releases) and open it.
Android will ask permission to install from your browser or file manager the
first time; that prompt is the only check there is on a sideloaded app.

## Updating

The app checks here once a day and offers anything newer. There is also a
manual check under **Settings → App version**.

## Why this is separate from the desktop releases

The desktop app updates through electron-updater, which reads whichever
release GitHub marks as *latest* and expects a `latest.yml` inside it. An
Android release published alongside the desktop ones would become *latest*,
carry no `latest.yml`, and silently stop every gym's desktop app from
updating. Keeping the two apart is what prevents that.
