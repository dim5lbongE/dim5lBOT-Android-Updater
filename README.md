# dim5lBOT Updater for Android

Checks the official dim5lBOT update manifest on launch, verifies downloads with SHA-256, and replaces the installed Geode package through Android's persisted Storage Access Framework permission.

On first launch, select the mods folder through either Android storage or
Geode Launcher's user-directory document provider:

`Android/media/com.geode.launcher/game/geode/mods`

The updater stages and verifies the complete package before replacing the old
file, restores the previous package if replacement fails, and validates the
embedded mod ID, version, and Android64 binary.
