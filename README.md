# SQUABIX Node Saving

Save and load node properties. Nodes in the scene and nodes made at runtime both work.

## Classes

- `NodeSaver`
- `NodeSave`
- `Save`

## Use

1. Add a `NodeSaver` under each node you want to save.
2. Pick the properties in `saved_properties`.
3. Set `NodeSaver.scene_root` to your level and `NodeSaver.save` to a `Save`.
4. Call `NodeSaver.save_all()`, then `Save.write_to_disk()`.
5. To load, call `Save.load_from_disk()`, set `NodeSaver.save`, then call `NodeSaver.load_all()`.

Extend `Save` to add your own data.

## Demo

See it in the game: https://github.com/squabix/craftlander

## Needs

Godot 4.5 or newer.

## License

MIT. See `LICENSE`.
Icons are from another project. See `THIRD_PARTY.md`.
