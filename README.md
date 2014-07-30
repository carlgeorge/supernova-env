# supernova-env

Bootstrap a complete supernova environment using virtualenv.

## Installation

Just download the script and put it in your path somewhere.

```
MYSCRIPTS=~/.local/share/bin
wget -P ${MYSCRIPTS} https://raw.github.com/cgtx/supernova-env/master/supernova-env
chmod +x ${MYSCRIPTS}/supernova-env
```

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
    $ mv ~/.config/supernova{.sample,}
    $ vim ~/.config/supernova
    <--- edit the config as necessary --->
