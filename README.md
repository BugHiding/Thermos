# Cauldron 

![Minecraft Forge v10.13.4.1614][forge]
![Minecraft v1.7.10][mc]
![Java JDK v1.8][java]
![Spigot 1.7.10 Snapshot ][spigot]

### Continuation of KCauldron minecraft server

This github was created due to the previous developer for KCauldron being missing for weeks - sometimes months - at a time.  When the dev was missing his gitlab would go offline making it "feel" like the project was abandoned completely.

This repo was based on KCauldron 1492 Build 152.  Some extra patches were added and cherry picked in order to improve and fix up some of the small little flaws that were inherent in the 152 build.

## Chat

Feel free to drop in on the Discord chat [here](https://discord.gg/0VmBoNh2sE2t5yKh)

## Issues

There won't be any support given for making mods work with this particular repo of KCauldron.  Blame the stupid people that can't read.

Basically;

**I will not give support or patch updates or fixes on this repo for mods to work. This fork is put together by the community by submitting their own pull requests, Yive does not know Java nor does he want to learn it to work on this fork.**

## Contributing

Please read the [guide](https://github.com/TCPR/KCauldron/blob/master/CONTRIBUTING.md) on how to contribute - Cauldron always needs improvements :smile: 

## Downloads
You can download the pre-built packages from [here](https://tcpr.ca/downloads/kcauldron)
I'd suggest that you look at the release notes before downloading.


## Build Requirements
* Java 8 JDK
* `JAVA_HOME` defined on your OS

## Building Cauldron
* Checkout project
  * You can use IDE or clone from console:
  `git clone https://github.com/TCPR/KCauldron.git`
* Init submodules
  * Since this project uses two other projects we need to download them as well
  `git submodule update --init --recursive`
* Start build process
  * This process downloads minecraft and apply patches
  * If you have gradle integration in IDE - you can still use gui
  `./gradlew setupCauldron jar`

All builds will be in `build/distributions`
  
## Updating sources
* Update sources
  * `git pull origin master`
* Re apply patches & build binaries
  * `./gradlew clean setupCauldron jar`

[forge]: https://img.shields.io/badge/Minecraft%20Forge-v10.13.4.1614-green.svg "Minecraft Forge v10.13.4.1614"
[mc]: https://img.shields.io/badge/Minecraft-v1.7.10-green.svg "Minecraft 1.7.10"
[java]: https://img.shields.io/badge/Java%20JDK-v1.8-blue.svg "Java JDK 8"
[spigot]: https://img.shields.io/badge/Spigot-v1.7.10--R0.1--SNAPSHOT-lightgrey.svg "Spigot R0.1 Snapshot"
