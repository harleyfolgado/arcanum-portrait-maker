# Release Checklist

- [ ] Confirm public docs contain no local machine paths.
- [ ] Confirm no source tree, test install, scratch data, reports, or restore folders are included.
- [ ] Confirm no Arcanum executable, DAT archives, DLLs, WorldEd, Factory tools, or copied game install folders are included in the repo export.
- [ ] Confirm release asset was built from the latest app.
- [ ] Confirm release asset was scanned before upload.
- [ ] Confirm `ArcanumPortraitMaker-v1.0.0-win32-x64.zip` is uploaded as a GitHub Release asset on tag `v1.0.0-starter-pack`.
- [ ] Confirm the 172 MB ZIP was not committed to the git repo as a normal blob.
- [ ] Confirm the published SHA256 is `5B2EAD1756679BC14CE6DDC43F69560A7246CA47AFDF528E89051466DEB91984`.
- [ ] Confirm Starter Character Pack preview reports `12 / 12` on a throwaway install.
- [ ] Launch Arcanum manually and click through all 12 Pick Character slots.
- [ ] Start Sir Rogers, Elias, Mara, and one small-race character.
- [ ] Verify starter inventories.
- [ ] Verify Create Character does not show Starter Character Pack leakage.
- [ ] Test Restore Stock Characters.
- [ ] Reinstall after restore.
