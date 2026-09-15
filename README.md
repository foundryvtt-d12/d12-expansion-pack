# D12 Expansion Pack

A shareable compendium module for the [D12 system](https://github.com/foundryvtt-d12/d12) in Foundry Virtual Tabletop. It ships an additional compendium of NPCs and monsters, to expand on [D12 Core Content](https://github.com/foundryvtt-d12/d12-core-content).

## Installation

Requires the D12 system to be installed. In Foundry's **Add-on Modules** install screen, use this manifest URL:

```
https://github.com/foundryvtt-d12/d12-expansion-pack/releases/latest/download/module.json
```

Then enable "D12 Expansion Pack" in your world's module settings.

## Contents

- **D12 Expansion NPCs** — ready-to-drop non-player characters and monsters.

## Contributing content

Compendium content is authored as plain JSON files under `packs/_source/`, one file per document, and compiled into Foundry's compendium format for distribution.

```
npm install       # install dependencies
npm run build     # compile packs/_source/** into packs/<name>/ (LevelDB)
npm run unpack    # re-export compiled packs back into packs/_source/** (after live edits in Foundry)
```

To edit content locally:

1. Run `npm run build`.
2. Symlink this repository folder into your Foundry `Data/modules/d12-expansion-pack` folder.
3. Enable the module in a D12 world, then either:
   - Edit the JSON files under `packs/_source/` directly and re-run `npm run build`, then use Foundry's "Reload All Compendiums", or
   - Unlock a compendium in Foundry and edit it live, then run `npm run unpack` to bring the changes back into `packs/_source/` for review and commit.

## License

Licensed under [CC BY-NC 4.0](LICENSE).

Third-party artwork credits are listed in [ATTRIBUTIONS.md](ATTRIBUTIONS.md).
