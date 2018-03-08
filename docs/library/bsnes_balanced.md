# Nintendo - SNES / Famicom (bsnes Balanced)

## Background

bsnes is a Super Nintendo emulator that began development on 2004-10-14. It focuses on accuracy and clean code above all else. It never uses speed or compatibilty hacks. As a result, the minimum system requirements are greater than with other emulators. bsnes comes in three different profiles (accuracy, balanced and performance) which contain minor differences in the PPU (graphics) emulation. 

This core has been compiled with the Balanced profile.

Highly accurate SNES emulation. Whether to use the Accuracy, or Balanced or Performance core depends on how much accuracy you want to give up for game performance. 

Please check the [compatibility section](https://docs.libretro.com/library/bsnes_balanced/#compatibility) for more information.

### Author/License

The bsnes Balanced core has been authored by

- byuu

The bsnes Balanced core is licensed under

- [GPLv3](https://github.com/libretro/bsnes-libretro/blob/libretro/COPYING)

A summary of the licenses behind RetroArch and its cores have found [here](https://docs.libretro.com/tech/licenses/).

## Extensions

Content that can be loaded by the bsnes Balanced core have the following file extensions:

- .sfc
- .smc
- .bml

## Databases

RetroArch database(s) that are associated with the bsnes Balanced core:

- [Nintendo - Super Nintendo Entertainment System](https://github.com/libretro/libretro-database/blob/master/rdb/Nintendo%20-%20Super%20Nintendo%20Entertainment%20System.rdb)
- [Nintendo - Super Nintendo Entertainment System Hacks](https://github.com/libretro/libretro-database/blob/master/rdb/Nintendo%20-%20Super%20Nintendo%20Entertainment%20System%20Hacks.rdb)
- [Nintendo - Sufami Turbo](https://github.com/libretro/libretro-database/blob/master/rdb/Nintendo%20-%20Sufami%20Turbo.rdb)

## BIOS

Required or optional firmware files go in the frontend's system directory.

!!! attention
	The bsnes Balanced core uses split ROMS for [special chip games](https://en.wikipedia.org/wiki/List_of_Super_NES_enhancement_chips#List_of_Super_NES_games_that_use_enhancement_chips).

Notable DSP1/DSP1B Games: 

- Super Mario Kart
- Pilotwings

Notable DSP2 Games:

- Dungeon Master

Notable DSP3 Games:

- SD Gundam GX

Notable DSP4 Games: 

- Top Gear 3000

Notable Cx4 Games:

- Mega Man X2
- Mega Man X3

| Filename          | Description                            | md5sum                           |
|:-----------------:|:--------------------------------------:|:--------------------------------:|
| dsp1.data.rom     | DSP1 co-processor firmware             | 3d81b45fa0c2aa8b852dfb1ece7c0971 |
| dsp1.program.rom  | DSP1 co-processor firmware             | ae209fbe789fbf11a48aea5ab1197321 |
| dsp1b.data.rom    | DSP1B co-processor firmware            | 1e3f568634a7d8284020dddc0ae905bc |
| dsp1b.program.rom | DSP1B co-processor firmware            | d10f446888e097cbf500f3f663cf4f6d |
| dsp2.data.rom     | DSP2 co-processor firmware             | e9417e29223b139c3c4b635a2a3b8744 |
| dsp2.program.rom  | DSP2 co-processor firmware             | aa6e5922a3ed5ded54f24247c11143c5 |
| dsp3.data.rom     | DSP3 co-processor firmware             | 0a81210c0a940b997dd9843281008ee6 |
| dsp3.program.rom  | DSP3 co-processor firmware             | d99ca4562818d49cee1f242705bba6f8 |
| dsp4.data.rom     | DSP4 co-processor firmware             | ee4990879eb68e3cbca239c5bc20303d |
| dsp4.program.rom  | DSP4 co-processor firmware             | a151023b948b90ffc23a5b594bb6fef2 |
| cx4.data.rom      | CX4 co-processor firmware              | 037ac4296b6b6a5c47c440188d3c72e3 |
| st010.data.rom    | ST010 co-processor firmware            | 254d70762b6f59f99c27c395aba7d07d |
| st010.program.rom | ST010 co-processor firmware            | 1d70019179a59a566a0bb5d3f2845544 |
| st011.data.rom    | ST011 co-processor firmware            | 10bd3f4aa949737ab9836512c35bcc29 |
| st011.program.rom | ST011 co-processor firmware            | 95222ebf1c0c2990bcf25db43743f032 |
| st018.data.rom    | ST018 co-processor firmware            | 49c898b60d0f15e90d0ba780dd12f366 |
| st018.program.rom | ST018 co-processor firmware            | dda40ccd57390c96e49d30a041f9a9e7 |
| sgb.boot.rom      | Super Game Boy BIOS                    |                                  |

## Features

Frontend-level settings or features that the bsnes Balanced core respects.

| Feature           | Supported |
|-------------------|:---------:|
| Restart           | ✔         |
| Screenshots       | ✔         |
| Saves             | ✔         |
| States            | ✔         |
| Rewind            | ✔         |
| Netplay           | ✔         |
| Core Options      | ✕         |
| RetroAchievements | ✔         |
| RetroArch Cheats  | ✔         |
| Native Cheats     | ✕         |
| Controls          | ✔         |
| Remapping         | ✔         |
| Multi-Mouse       | -         |
| Rumble            | ✕         |
| Sensors           | ✕         |
| Camera            | ✕         |
| Location          | ✕         |
| Subsystem         | ✔         |
| [Softpatching](https://docs.libretro.com/guides/softpatching/) | ✔         |
| Disk Control      | ✕         |
| Username          | ✕         |
| Language          | ✕         |
| Crop Overscan     | ✔         |
| LEDs              | ✕         |

### Directories

The bsnes Balanced core's internal core name is 'bsnes'

The bsnes Balanced core saves/loads to/from these directories.

**Frontend's Save directory**

- 'content-name'.srm (Cartridge battery save)

**Frontend's State directory**

- 'content-name'.state# (State)

### Geometry and timing

- The bsnes Balanced core's core provided FPS is 60.0988118623 for NTSC games and 50.0069789082 for PAL games.
- The bsnes Balanced core's core provided sample rate is 32040.5 Hz
- The bsnes Balanced core's core provided aspect ratio is 4/3

## Super GameBoy

!!! warning
	Super GameBoy support in this core is **Windows only**, and has **buggy save state support** and **visual glitches**. **Use the [higan Accuracy core](https://docs.libretro.com/library/higan_accuracy#super-gameboy-support) or the [nSide Balanced core](https://docs.libretro.com/library/nside_balanced#super-gameboy-support) for simplified, functional, and easily accessible Super Gameboy support.**

For Super GameBoy support, you need sgb.boot.rom (in RetroArch's System directory), a GameBoy ROM and a Super GameBoy ROM.

Please note that the Game Boy and Super GameBoy ROMs have to be unzipped.
	
Super GameBoy is supported via the Subsystem API.

There are two ways to access the Subsystem API.

**One way is to access the Subsystem API through RetroArch's GUI like this.**

First, we load our GameBoy ROM through 'Load Super GameBoy' in RetroArch's Main Menu.

![](../image/core/bsnes/menu1.png)

![](../images/core/bsnes/gb.png)

Next, we load our Super GameBoy ROM through 'Load Super GameBoy' in RetroArch's Menu Menu.

![](../image/core/bsnes/menu2.png)

![](../image/core/bsnes/sgb.png)

Then, we start the content by selecting 'Start GameBoy' In RetroArch's Menu Menu.

![](../image/core/bsnes/start.png)

**The other way is to launch RetroArch with commandline like this.**

```
retroarch -L {path to bsnes core} {path to Super GameBoy ROM} --subsystem sgb {path to GameBoy rom}
```

## MSU-1

!!! attention
	MSU-1 support in this core is complex. **Use the [Snes9x core](https://docs.libretro.com/library/snes9x#msu-1-support) for simplified and easily accessible MSU-1 support.**

MSU-1 support can be used by loading a correct .bml file.

There's documentation for loading MSU-1 games in standalone higan [here](https://higan.readthedocs.io/en/stable/guides/import/#msu-1-games).
	
## Controllers

The bsnes Balanced core supports the following device type(s) in the controls menu, bolded device types are the default for the specified user(s):

### User 1 device types

- None - Disables input.
- **[SNES Joypad](http://nintendo.wikia.com/wiki/Super_Nintendo_Entertainment_System_controller)** - Joypad
- [SNES Mouse](https://en.wikipedia.org/wiki/Super_NES_Mouse) - Mouse

### User 2 device types

- None - Disables input.
- **[SNES Joypad](http://nintendo.wikia.com/wiki/Super_Nintendo_Entertainment_System_controller)** - Joypad
- [SNES Mouse](https://en.wikipedia.org/wiki/Super_NES_Mouse) - Mouse
- [Multitap](http://nintendo.wikia.com/wiki/Super_Multitap) - Joypad - Allows for up to five players to play together in multitap games.
- [SuperScope](https://en.wikipedia.org/wiki/Super_Scope) - Lightgun
- [Justifier](https://en.wikipedia.org/wiki/Konami_Justifier) - Lightgun
- [Justifiers](https://en.wikipedia.org/wiki/Konami_Justifier) - Lightgun - Two Justifiers are plugged in, for two-player Justifier games.

### Multitap support

Activating multitap support in compatible games can be configured by switching to the [Multitap device type](https://docs.libretro.com/library/bsnes_balanced#controllers) for User 2.

### Controller tables

#### Joypad

![](../image/controller/snes.png)

| User 1 - 5 Remap descriptors | RetroPad Inputs                           |
|------------------------------|-------------------------------------------|
| B                            | ![](../image/retropad/retro_b.png)    |
| Y                            | ![](../image/retropad/retro_y.png)    |
| Select                       | ![](../image/retropad/retro_select.png)     |
| Start                        | ![](../image/retropad/retro_start.png)      |
| D-Pad Up                     | ![](../image/retropad/retro_dpad_up.png)    |
| D-Pad Down                   | ![](../image/retropad/retro_dpad_down.png)  |
| D-Pad Left                   | ![](../image/retropad/retro_dpad_left.png)  |
| D-Pad Right                  | ![](../image/retropad/retro_dpad_right.png) |
| A                            | ![](../image/retropad/retro_a.png)    |
| X                            | ![](../image/retropad/retro_x.png)    |
| L                            | ![](../image/retropad/retro_l1.png)         |
| R                            | ![](../image/retropad/retro_r1.png)         |

#### Mouse

| RetroMouse Inputs                                   | SNES Mouse                |
|-----------------------------------------------------|---------------------------|
| ![](../image/retromouse/retro_mouse.png) Mouse Cursor | SNES Mouse Cursor         |
| ![](../image/retromouse/retro_left.png) Mouse 1       | SNES Mouse Left Button    |
| ![](../image/retromouse/retro_right.png) Mouse 2      | SNES Mouse Right Button   |

#### Lightgun

| RetroLightgun Inputs                                 | SuperScope                | Justifier(s)        |
|------------------------------------------------------|---------------------------|---------------------|
| ![](../image/retromouse/retro_mouse.png) Gun Crosshair | SuperScope Crosshair      | Justifier Crosshair |
| Gun Trigger                                          | SuperScope Trigger        | Justifier Trigger   |
| Gun Aux A                                            | SuperScope Cursor         |                     |
| Gun Aux B                                            | SuperScope Turbo          |                     |
| Gun Start                                            | SuperScope Pause          | Justifier Start     |

## Compatibility

| Game                     | Issue                                                                          |
|--------------------------|--------------------------------------------------------------------------------|
| A.S.P. Air Strike Patrol | Black lines show up during gameplay. The shadow below the aircraft is missing. |

## External Links

- [Official higan Website](https://byuu.org/)
- [Official higan Upstream Downloads](https://byuu.org/emulation/higan/)
- [Libretro bsnes Balanced Core info file](https://github.com/libretro/libretro-super/blob/master/dist/info/bsnes_balanced_libretro.info)
- [Libretro bsnes Balanced Github Repository](https://github.com/libretro/bsnes-libretro)
- [Report Libretro bsnes Balanced Core Issues Here](https://github.com/libretro/bsnes-libretro/issues)

### See also

#### Nintendo - Sufami Turbo

- [Nintendo - SNES / Famicom (Beetle bsnes)](https://docs.libretro.com/library/beetle_bsnes/)
- [Nintendo - SNES / Famicom (bsnes-mercury Accuracy)](https://docs.libretro.com/library/bsnes_mercury_accuracy/)
- [Nintendo - SNES / Famicom (bsnes-mercury Balanced)](https://docs.libretro.com/library/bsnes_mercury_balanced/)
- [Nintendo - SNES / Famicom (bsnes-mercury Performance)](https://docs.libretro.com/library/bsnes_mercury_performance/)
- [Nintendo - SNES / Famicom (bsnes Accuracy)](https://docs.libretro.com/library/bsnes_accuracy/)
- [Nintendo - SNES / Famicom (bsnes C++98 (v085))](https://docs.libretro.com/library/bsnes_cplusplus98/)
- [Nintendo - SNES / Famicom (bsnes Performance)](https://docs.libretro.com/library/bsnes_performance/)
- [Nintendo - SNES / Famicom (Snes9x)](https://docs.libretro.com/library/snes9x/)
- [Nintendo - SNES / Famicom (Snes9x 2002)](https://docs.libretro.com/library/snes9x_2002/)
- [Nintendo - SNES / Famicom (Snes9x 2005 Plus)](https://docs.libretro.com/library/snes9x_2005_plus/)
- [Nintendo - SNES / Famicom (Snes9x 2005)](https://docs.libretro.com/library/snes9x_2005/)
- [Nintendo - SNES / Famicom (Snes9x 2010)](https://docs.libretro.com/library/snes9x_2010/)

#### Nintendo - Super Nintendo Entertainment System (+ Hacks)

- [Nintendo - SNES / Famicom (Beetle bsnes)](https://docs.libretro.com/library/beetle_bsnes/)
- [Nintendo - SNES / Famicom (bsnes-mercury Accuracy)](https://docs.libretro.com/library/bsnes_mercury_accuracy/)
- [Nintendo - SNES / Famicom (bsnes-mercury Balanced)](https://docs.libretro.com/library/bsnes_mercury_balanced/)
- [Nintendo - SNES / Famicom (bsnes-mercury Performance)](https://docs.libretro.com/library/bsnes_mercury_performance/)
- [Nintendo - SNES / Famicom (bsnes Accuracy)](https://docs.libretro.com/library/bsnes_accuracy/)
- [Nintendo - SNES / Famicom (bsnes C++98 (v085))](https://docs.libretro.com/library/bsnes_cplusplus98/)
- [Nintendo - SNES / Famicom (bsnes Performance)](https://docs.libretro.com/library/bsnes_performance/)
- [Nintendo - SNES / Famicom (higan Accuracy)](https://docs.libretro.com/library/higan_accuracy/)
- [Nintendo - SNES / Famicom (nSide Balanced)](https://docs.libretro.com/library/nside_balanced/)
- [Nintendo - SNES / Famicom (Snes9x)](https://docs.libretro.com/library/snes9x/)
- [Nintendo - SNES / Famicom (Snes9x 2002)](https://docs.libretro.com/library/snes9x_2002/)
- [Nintendo - SNES / Famicom (Snes9x 2005 Plus)](https://docs.libretro.com/library/snes9x_2005_plus/)
- [Nintendo - SNES / Famicom (Snes9x 2005)](https://docs.libretro.com/library/snes9x_2005/)
- [Nintendo - SNES / Famicom (Snes9x 2010)](https://docs.libretro.com/library/snes9x_2010/)