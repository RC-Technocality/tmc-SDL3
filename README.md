# The Legend of Zelda: The Minish Cap - Cross-Platform SDL3 Rework

This project is built off [The Legend of Zelda: The Minish Cap Decompilation] done by the Zelda Reverse Engineering Team.

My goal is to build upon this decompolation to create a version of The Legend of Zelda: The Minish Cap that can be run as an application on various platforms, 
using [Simple DirectMedia Layer] (specifically SDL3) as a backend.

In order for the application to function, a user must provide their own copy of The Legend of Zelda: The Minish Cap (USA) as a rom image.
The application is not built off anything other than the decompilation of the game, which does not include the game's assets. The rom image is the means by which the application
accesses these assets (sprites, music, etc).

My project does not condone nor enable piracy. The Legend of Zelda: The Minish Cap is a commercially available game, and shall not be provided with this application.

[The Legend of Zelda: The Minish Cap Decompilation]: https://github.com/zeldaret/tmc.git
[Simple DirectMedia Layer]: https://github.com/libsdl-org/SDL.git











# The Legend of Zelda: The Minish Cap


[![Build Status][jenkins-badge]][jenkins] [![Decompilation Progress][progress-badge]][progress] [![Contributors][contributors-badge]][contributors] [![Discord Channel][discord-badge]][discord]

[jenkins]: https://jenkins.deco.mp/job/TMC/job/master
[jenkins-badge]: https://img.shields.io/jenkins/build?jobUrl=https%3A%2F%2Fjenkins.deco.mp%2Fjob%2FTMC%2Fjob%2Fmaster

[progress]: https://zelda64.dev/games/tmc
[progress-badge]: https://img.shields.io/endpoint?url=https://zelda64.dev/assets/csv/progress-tmc-shield.json

[contributors]: https://github.com/zeldaret/tmc/graphs/contributors
[contributors-badge]: https://img.shields.io/github/contributors/zeldaret/tmc

[discord]: https://discord.zelda64.dev
[discord-badge]: https://img.shields.io/discord/688807550715560050?color=%237289DA&logo=discord&logoColor=%23FFFFFF

```diff
- WARNING! -

This repository is a work in progress, and while it can be used to make certain changes, it's still
constantly evolving. If you use it for modding purposes in its current state, please be aware that
the codebase can drastically change at any time. Also note that some parts of the ROM may not be
'shiftable' yet, so modifying them could be difficult at this point.
```

This is a WIP decompilation of The Legend of Zelda: The Minish Cap.
The purpose of the project is to recreate a source code base for the game from scratch, using information found inside the game along with static and/or dynamic analysis.

It can target the following ROMs:

* [**tmc.gba**](https://datomatic.no-intro.org/index.php?page=show_record&s=23&n=1841) `sha1: b4bd50e4131b027c334547b4524e2dbbd4227130`
* [**tmc_jp.gba**](https://datomatic.no-intro.org/index.php?page=show_record&s=23&n=1719) `sha1: 6c5404a1effb17f481f352181d0f1c61a2765c5d`
* [**tmc_eu.gba**](https://datomatic.no-intro.org/index.php?page=show_record&s=23&n=1734) `sha1: cff199b36ff173fb6faf152653d1bccf87c26fb7`
* [**tmc_demo_usa.gba**](https://datomatic.no-intro.org/index.php?page=show_record&s=23&n=x051) `sha1: 63fcad218f9047b6a9edbb68c98bd0dec322d7a1`
* [**tmc_demo_jp.gba**](https://datomatic.no-intro.org/index.php?page=show_record&s=23&n=x430) `sha1: 9cdb56fa79bba13158b81925c1f3641251326412`

**Note:** This repository does not include any of the assets necessary to build the ROM.
A prior copy of the game is required to extract the needed assets.

Website: <https://zelda64.dev>

Discord: <https://discord.zelda64.dev>

Documentation: <https://zeldaret.github.io/tmc>

## Installation

To set up the repository, see [INSTALL.md](INSTALL.md).

## Contributing

All contributions are welcome. This is a group effort, and even small contributions can make a difference.
Some tasks also don't require much knowledge to get started.

Most discussions happen on our [Discord Server](https://discord.zelda64.dev), where you are welcome to ask if you need help getting started, or if you have any questions regarding this project and other decompilation projects.
