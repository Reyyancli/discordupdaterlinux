# Linux Discord Updater
Small script that updates discord for you if you have installed it in `/opt`
This does **not** install discord for you (yet). It is meant to update the files in `/opt`

The script caches the downloaded tar.gz files in `$HOME/.config/discord-updates`
#### Note
This is my first actual script so if something is not right or not working, please open an issue about it
## Usage
You can run the script standalone and it will update your discord
If you run `./discord-update install` it will install the script *(put it in the `/usr/bin/` directory for easy access)*

To run the script you may need to add executable permissions
```
sudo chmod +x <filename or filepath>
```
### Available commands
`-h` : Shows the available options
`-v, --vencord` : Runs the vencord installer script
`--clean` : Clean the cache built up in `$HOME/.config/discord-updates`. Does not delete anything else that may be in the directory unless specifically named `discord-(anything here).tar.gz`
