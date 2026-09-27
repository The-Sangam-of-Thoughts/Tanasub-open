# Aider conventions adapter

## Load

From the repository root, start Aider with this file and the router as read-only context:

```shell
aider --read platform-adapters/aider-conventions.md --read SKILL.md
```

In an existing chat, use `/read platform-adapters/aider-conventions.md` and `/read SKILL.md`. Aider also supports persistent `read:` entries in `.aider.conf.yml`. These are the documented mechanisms in [Specifying coding conventions](https://aider.chat/docs/usage/conventions.html); `.aider/conventions.md` is not a documented automatic convention path.

## Convention

Follow `SKILL.md`. Read one matching Layer 0 file with `/read`, then only the optional layer and single genre or subgenre file needed for the task. Add a deeper reference only for a specific unresolved question. Do not load the repository wholesale. Minimize context, but never use a hard token cap to omit evidence, constraints, accessibility, or necessary craft detail. Keep Aider output review separate from platform acceptance.
