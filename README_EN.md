# YueXinMiao 2 Codex Desktop Pet
[中文 README](README.md) | [English README](README_EN.md)

This repository contains a local Codex desktop pet package named **月薪猫2**.
The spritesheet is organized in the Codex 9-row standard animation format.

![YueXinMiao 2 animation preview](assets/preview-standard-actions.png)

## Contents

| File | Description |
| --- | --- |
| `pet.json` | Codex pet manifest containing the pet name, description, and spritesheet path. |
| `spritesheet.png` | The installable animation atlas, sized `1536 x 1872`. |
| `assets/preview-standard-actions.png` | Static frame preview for all 9 standard animation rows. |
| `NOTICE.md` | Source and attribution notes. |
| `LICENSE-NOTE.md` | Licensing and redistribution reminder. |
| `CONTRIBUTING.md` | Notes for people who want to modify the pet package. |

## Standard Animations

This package contains 9 standard animations:

| Row | State | Description | Frames |
| ---: | --- | --- | ---: |
| 0 | `idle` | Idle | 6 |
| 1 | `running-right` | Moving right | 8 |
| 2 | `running-left` | Moving left | 8 |
| 3 | `waving` | Waving | 4 |
| 4 | `jumping` | Jumping | 5 |
| 5 | `failed` | Failed or error reaction | 8 |
| 6 | `waiting` | Waiting for user input | 6 |
| 7 | `running` | Actively working | 6 |
| 8 | `review` | Reviewing or checking | 6 |

## Changes In This Version

- Preserves the main YueXinMiao 2 character and animation set.
- Replaces the `waiting` row with the `waiting` animation from the local 月薪猫 pet.
- Uses PNG for the final atlas so transparent pixels remain clean.
- The atlas was checked locally for the expected `1536 x 1872` size, 8-column x 9-row layout, and transparent background.

## Installation

### Option 1: Copy the pet folder

1. Download this repository.
2. Copy the repository contents into:

```text
~/.codex/pets/yuexinmiao-2
```

3. Confirm that the directory contains:

```text
~/.codex/pets/yuexinmiao-2/
├── pet.json
└── spritesheet.png
```

4. Restart Codex or switch pets once so the local pet is reloaded.

### Option 2: Install from the command line

Run these commands from the repository directory:

```bash
mkdir -p ~/.codex/pets/yuexinmiao-2
cp pet.json spritesheet.png ~/.codex/pets/yuexinmiao-2/
```

Then restart Codex or switch pets once.

## Troubleshooting

If the pet does not appear in Codex, check the following:

1. Both `pet.json` and `spritesheet.png` are inside `~/.codex/pets/yuexinmiao-2/`.
2. `pet.json` points to `spritesheet.png`.
3. Codex has been restarted, or the pet has been switched once.
4. The spritesheet size is `1536 x 1872`.

## Intended Use

This package is intended for sharing with people who use Codex desktop pets
and know how to install a local pet package.

## Artwork and Licensing

This repository packages local pet files for convenience. See `NOTICE.md` for
source and attribution notes. Before public redistribution, commercial use,
or derivative work, verify the permissions for the upstream artwork and
original character.

## Language

- [中文说明](README.md)
