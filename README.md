# Single line NMR Pipe installation

```sh
wget -qO- https://raw.githubusercontent.com/eburakova/nmrpipe-automatic-installation/master/nmrpipe-ubuntu-install.sh | bash
```

Takes care of downolading, all dependancies and the post-installation modifications of the ~/.cshrc file.

Bourne shell script to install [NMRPipe](https://spin.niddk.nih.gov/bax/NMRPipe/) on Ubuntu 22.04 Jammy.

The script tries to install NMRPipe on Ubuntu 22.04 in an automatic fashion by first downloading the
archives and scripts (if they are not downloaded yet) and then installing them.

## Requirements
* Ubuntu 22.04.4 LTS
* Admin rights

## Flow
1. Creates a folder `tmp_download` in the current directory
2. Checks if the necessary files already exist and downloads them, if necessary
3. Creates the installation directory: `/opt/nmrpipe` (here you'll have to type your admin password)
4. Copies the installation scripts there and executes the `install.com`
5. Modifes the `~/.cshrc` file as directed in README_NMRPIPE_USERS
6. Prompts user to remove the `tmp_download` folder with the source archives.

Simple as that!




