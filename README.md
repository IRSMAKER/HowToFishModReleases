# How to Fish - Mod Releases

Binary releases for the mods listed in the How to Fish mod catalogue.

**Do not add files here by hand.** The DLLs are published by the catalogue tooling in the
[HowToFishMods](https://github.com/IRSMAKER/HowToFishMods) repository, which verifies each
file's SHA-512 against `catalog.json` before uploading:

```
.\tools\Publish-Mod.ps1 -Slug <slug> -VersionNumber <x.y.z> -Provider GitHub -Repo IRSMAKER/HowToFishModReleases
```

Each release tag (`v1.0.0`, `v1.1.0`, ...) holds the built mod for that version. The
catalogue records the download URL and the expected hash, and the installer refuses to install
anything that does not match.

Players download through the installer app, not from here directly.
