# Forge Launcher data

What the Forge Launcher reads from the internet:

- `launcher.json` and `launcher.json.sig`: the FORGE servers, the HogwartsMP build they run, and the news.
  The file is signed; a launcher ignores a copy that was changed by anyone else.
- `mods.json`: the CurseForge mods of every server without a list of its own, and the list launchers before 0.6.0 use for every server.
- `mods-br.json`, `mods-ita.json`: a server's own mod list (launcher 0.6.0 and newer). A server names it with `"modsFile"` in the servers file given to `tools publish`, which writes its `"modsSha256"` into `launcher.json` itself: never edit that by hand. Commit the lists together with `launcher.json`, `launcher.json.sig` and `mods.json`.
- Releases: the launcher's setup file and its updates.

Players do not need anything from this page except the setup file under **Releases**.

Not affiliated with Warner Bros. Games, Avalanche Software, MafiaHub or CurseForge. You must own Hogwarts Legacy.
