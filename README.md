# Template for Forge 1.8.9 + Mixins

**Note:** I have only tested this with IntelliJ, but it should work with Eclipse just fine.

## Introduction

This repository includes a plug-and-play project template for 1.8.9 Forge Development with Mixins.

It contains an example mod with an example mixin (`MixinMinecraft.java`).

## Setup

1. Download or clone this repository
2. Open it as a Project
3. The gradle setup should be running automatically, if not, use `./gradlew`
4. Run the gradle task `gradle setupDecompWorkspace` (if you are getting the error "Heap Memory too low", increase the memory by adding `-Xmx4G` or `-Xmx8G` to the gradle task, depending on how much RAM you have; Right-Click the Gradle Task -> Modify Run Configuration... -> Modify Options -> Add VM Options)
5. If the setup is done, try to run the client with the example mod (use my prebuilt task `gradle buildCopyToRunModsAndRun` if you want -> combines building, copying to the run mods folder and running)
6. Nice! You just setup your working environment for 1.8.9 Forge Development with Mixins! If everything worked correctly you should find the following three things in your console:
   1. `[ExampleMod] Injecting with IFMLLoadingPlugin.`
   2. `Mixin worked!`
   3. `DIRT BLOCK >> tile.dirt`

## Post-Setup

Do the TODOs that are marked in:

- `build.gradle`
- `src/main/java/com/example/examplemod/mixins/MixinLoader.java`

Change the data in the `resources/mcmod.info` and rename and change the data of `resources/mixins.examplemod.json`

## Need help?

If you followed these steps but something went wrong, you can open an issue or contact me (see contact options on my profile), I am happy to help!

## License

You can read all the applying licenses in the file `LICENSE.md`

## Support

If you like this project, feel free to support me!<br><br>
[!["Buy Me A Coffee"](https://www.buymeacoffee.com/assets/img/custom_images/orange_img.png)](https://www.buymeacoffee.com/manuthebyte)
