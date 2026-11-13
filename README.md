# A repository to manage my personal config files

## Prerequisites
-  Have a pc.
-  Have `chezmoi` installed.
-  Yo configs normally sit inside of ~/.config/

## How to init

### The short way

```bash
chezmoi init --apply https://github.com/naaul1/dotfiles.git
```

### The precise way

```bash
chezmoi init https://github.com/naaul1/dotfiles.git   # clone this repo as the chezmoi's local repo
chezmoi apply                                         # copy files from chezmoi to ~/.config/
```

## Further use

```bash
chezmoi add path/to/file/config.file                  # have chezmoi track yo target config file
chezmoi edit path/to/file/config.file                 # edit the source of the target config file
chezmoi apply path/to/file/config.file                # apply a specific config file
chezmoi cd                                            # cd into chezmoi's local repo
                                                      # , can perform git actions from here
```
