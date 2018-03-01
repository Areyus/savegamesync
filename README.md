# Save Game Syncer with Owncloud/Nextcloud for Linux
A little script which syncs (uploads and downloads) savegames for common linux games.

## Currently supported Games
* AmnesiaADarkDescent
* Celeste
* Deponia1
* Deponia2
* Deponia3
* Guacamelee
* Hacknet
* Hedgewars
* HollowKnight
* HunieCamStudio
* HuniePop
* OlliOlli
* OlliOlli2
* Quake3
* ShovelKnight
* Skullgirls
* StardewValley
* SuperHexagon
* SuperMeatBoy
* Teeworlds
* TheEndIsNigh

## Configuration
Before you can use the script, you need a configuration file
in your home directory. Generate one with the setup wizard:
```bash
savegame_sync.sh -s [--setup]
```

## Usage
Upload the files to your Cloud:
```bash
savegame_sync.sh -u [--upload] --games "$Game1, $Game2"
```

Download the files from your Cloud
to the correct location:
```bash
savegame_sync.sh -d [--download] --games "$Game1, $Game2"
```

List all available games:
```bash
savegame_sync.sh -l [--list]
```

Wizard for the configuration file:
```bash
savegame_sync.sh -s [--setup]
```

Show the help message:
```bash
savegame_sync.sh -h [--help]
```

## ToDos
* save password hashed
* get password from stdin
* add functionality to up/download all with "all" string.
* Check several pathes for games.xml (/usr/share, /usr/local/share, $HOME/.local/share ./)
* prevent running the script as root
