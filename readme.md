Open QMK MSYS and cd to the root of this repo
```qmk compile -c -kb bastardkb/dilemma/3x5_2/splinky -km taipo```

# Quantum Mechanical Keyboard Firmware

For **the Dilemma 3x5_2**, it can be one of the following:

- `splinky`: for the [DIY version of the Dilemma](https://github.com/bastardkb/dilemma)
- `assembled`: for the [pre-assembled version of the Dilemma](https://bastardkb.com/dilemma/)

For **all other boards**, it can be one of the following:

- `v1/elitec`
- `v2/elitec`
- `v2/splinky_2`
- `v2/splinky_3`
- `v2/stemcell`
- `blackpill`

The version of the adapter can also be checked directly on the adapter PCB.

If you have any doubts, feel free to reach out for help on the [Discord](https://bastardkb.com/discord).

### Why `bkb-master` and `bkb-vial`

The changes on `bkb-master` are meant to be upstreamed and merged into QMK's `master` branch.

Vial, however, does not work out-of-the-box when using QMK's `master` branch, and relies instead of some changes that have not been upstreamed yet. Because of this, this repository trackes Vial's `master` branch (see below, `qmk-vial-head`) and cherry-picks Bastard Keyboards related changes on top of it.

Note that Vial's `master` usually lags a bit behind QMK's `master`, so the latest changes to QMK might not be available when working on `bkb-vial`.

## Feature branches

| Branch following QMK's `master` | Parent                     | Description                                          |
| ------------------------------- | -------------------------- | ---------------------------------------------------- |
| `bkb-master`                    | `qmk/qmk_firmware/master`  | Contains the latest sources for BastardKB's firmware |

| Branch following Vial's `master` | Parent          | Description                                        |
| -------------------------------- | ----------------| -------------------------------------------------- |
| `bkb-vial`                       | `qmk-vial-head` | Vial support on top of the changes in `bkb-master` |

# Quantum Mechanical Keyboard Firmware

[![Current Version](https://img.shields.io/github/tag/qmk/qmk_firmware.svg)](https://github.com/qmk/qmk_firmware/tags)
[![Discord](https://img.shields.io/discord/440868230475677696.svg)](https://discord.gg/Uq7gcHh)
[![Docs Status](https://img.shields.io/badge/docs-ready-orange.svg)](https://docs.qmk.fm)
[![GitHub contributors](https://img.shields.io/github/contributors/qmk/qmk_firmware.svg)](https://github.com/qmk/qmk_firmware/pulse/monthly)
[![GitHub forks](https://img.shields.io/github/forks/qmk/qmk_firmware.svg?style=social&label=Fork)](https://github.com/qmk/qmk_firmware/)

This is a keyboard firmware based on the [tmk\_keyboard firmware](https://github.com/tmk/tmk_keyboard) with some useful features for Atmel AVR and ARM controllers, and more specifically, the [OLKB product line](https://olkb.com), the [ErgoDox EZ](https://ergodox-ez.com) keyboard, and the [Clueboard product line](https://clueboard.co).

## Documentation

* [See the official documentation on docs.qmk.fm](https://docs.qmk.fm)

The docs are powered by [Docsify](https://docsify.js.org/) and hosted on [GitHub](/docs/). They are also viewable offline; see [Previewing the Documentation](https://docs.qmk.fm/#/contributing?id=previewing-the-documentation) for more details.

You can request changes by making a fork and opening a [pull request](https://github.com/qmk/qmk_firmware/pulls), or by clicking the "Edit this page" link at the bottom of any page.

## Supported Keyboards

* [Planck](/keyboards/planck/)
* [Preonic](/keyboards/preonic/)
* [ErgoDox EZ](/keyboards/ergodox_ez/)
* [Clueboard](/keyboards/clueboard/)
* [Cluepad](/keyboards/clueboard/17/)
* [Atreus](/keyboards/atreus/)

The project also includes community support for [lots of other keyboards](/keyboards/).

## Maintainers

QMK is developed and maintained by Jack Humbert of OLKB with contributions from the community, and of course, [Hasu](https://github.com/tmk). The OLKB product firmwares are maintained by [Jack Humbert](https://github.com/jackhumbert), the Ergodox EZ by [ZSA Technology Labs](https://github.com/zsa), the Clueboard by [Zach White](https://github.com/skullydazed), and the Atreus by [Phil Hagelberg](https://github.com/technomancy).

## Official Website

[qmk.fm](https://qmk.fm) is the official website of QMK, where you can find links to this page, the documentation, and the keyboards supported by QMK.
