# minecraft-json-schema

Updated to: Minecraft Java Edition 1.14

Json schemas for Minecraft files. Information about json schemas can be found at
[json-schema.org](http://json-schema.org/)

## Run Command

Loottable / Advancement Check

Specify the directory

```
LOOT_TABLE_JSON_DIR = ''
ADVANCEMENT_JSON_DIR = ''
```

python 2.7.15

1. `pip install jsonschema`
2. `cd ./script/`
3. `python validate_check.py`


CI Test Smple

https://travis-ci.com/TUSB/TheUnusualSkyBlock


## Design choices

-   The use of the `minecraft:` namespace is mandatory anywhere it can be used.
    This does mean that it will not necessarily validate against all vanilla
    files

## Current progress

At the moment, the following schemas are provided in the `java` folder:

1. Advancements
2. `pack.mcmeta` for both data and resource packs
3. `*.mcmeta` animation files
4. Loot tables
5. `sounds.json`
6. Models
7. Recipes

### Future plans

The following files should be supported in the future

1. Bedrock schemas

## License

<a rel="license" href="http://creativecommons.org/licenses/by/4.0/"><img alt="Creative Commons Licence" style="border-width:0" src="https://i.creativecommons.org/l/by/4.0/88x31.png" /></a><br />This
work is licensed under a
<a rel="license" href="http://creativecommons.org/licenses/by/4.0/">Creative
Commons Attribution 4.0 International License</a>.

Note that in `41a72f7` and earlier, the schemas were available under the
unlicense

### Projects known to be using this
