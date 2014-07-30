# supernova-env

Bootstrap a complete supernova environment using virtualenv.

## Installation

Just download the script and put it in your path.

```
MYSCRIPTS=~/.local/share/bin
wget -P ${MYSCRIPTS} https://raw.github.com/cgtx/supernova-env/master/supernova-env
chmod +x ${MYSCRIPTS}/supernova-env
```

By default, the script will put wrapper scripts in ~/.local/share/bin and put the virtualenv in ~/.local/share/virtualenv.  If you desire different paths, then modify the variables BIN_PATH and ENV_PATH within the script before running.

## Usage

    $ supernova-env
    usage:          supernova-env subcommand
    
    description:    Bootstrap a complete supernova environment using virtualenv.
    
    subcommands:    install     install the environment and wrapper scripts
                    upgrade     upgrade the pip pacakges in the environment
                    remove      remove the environment and wrapper scripts
                    template    create configuration template file
                    status      check the status of your installation

## Quickstart

    $ supernova-env install
    <--- script output --->
    $ supernova-env template > ~/.config/supernova
    $ vim ~/.config/supernova
    <--- edit the config as necessary --->
