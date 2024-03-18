<p align="center">
  <img src="https://raw.githubusercontent.com/UltimatChamp/CustomItemTextures/main/src/main/resources/assets/citresewn/logo.png" width="200px">
</p>

MCPatcher's CIT w/o OptiFine. A reliable fork of CITResewn!

The main CIT mod serves as an API to add types and conditions while CIT: Defaults uses that API to provide the default types and conditions that naturally come with the CIT format.

## Downloads
You can get CIT(bundled with Defaults) from Modrinth, CurseForge or by compiling it from source

              <a href="https://modrinth.com/mod/cit"><img src="https://citresewn.shcm.io/img/modrinth.png" width="50px"></a>       
<a href="https://www.curseforge.com/minecraft/mc-mods/cit-fork"><img src="https://citresewn.shcm.io/img/curseforge.png" width="50px"></a>

## CIT Docs
Docs for CIT Resewn's usage are available over at https://citresewn.shcm.io

## API

CIT is distributed for development through Modrinth's Maven repository under `cit`.<br>
Defaults can be added separately through the same Maven under `cit-resewn-defaults`.

Gradle example:
```groovy
// Add the modrinth maven repository:
repositories {
    ...
    maven {
        name = "Modrinth"
        url = "https://api.modrinth.com/maven"
        content {
            includeGroup "maven.modrinth"
        }
    }
}

dependencies {
    ...
    // Add the base CIT API to the project
    modCompileOnly "maven.modrinth:cit:1.0.0+1.20.4"
    // Add Defaults to the project
    modCompileOnly "maven.modrinth:cit-resewn-defaults:1.1.3+1.20"
}
```

API usage documentation will be available soon over at [the docs](https://citresewn.shcm.io/mods/mod_api/).

For example usage of the CIT API, take a look at how Defaults does it.

## Contributing

Bug fixes and feature implementations are always welcome and will usually be accepted once verified to be ok/fit in the mod.

Translations aren't really necessary but if you PR them there's no reason they won't be accepted.

Lastly, the docs site is also open source, PRs can be made to the [docs branch](https://github.com/SHsuperCM/CITResewn/tree/docs).

## Disclaimer
This is a temporary fork of **CITResewn**. The project will be archived, once the original mod is updated.
