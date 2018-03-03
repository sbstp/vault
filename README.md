# Vault
Easily track and backup configuration files.

Add files

```bash
$ vault add ~/.config/Code/User/settings.json # vscode settings
$ vault add /etc/fstab # mounts
```

List files

```bash
$ vault ls
/etc/fstab
/home/simon/.config/Code/User/settings.json
```

Backup files

```bash
$ vault backup laptop-backup.tar.gz
```

Restore files
```bash
$ vault restore laptop-backup.tar.gz
```

Usage
```
Usage: vault <command>

Commands:
  add      <path> [<path> ...]  Add files to the index.
  rm       <path> [<path> ...]  Remove files from the index.
  ls                            List files in the index.
  backup   <archive>            Backup files to an archive.
  restore  <archive>            Restores files from an archive.
  inspect  <archive>            List files, owner and mode information for an archive.
  extract  <archive> <dir>      Extract the contents of the archive to a directory.
  help     [<command>]          Display help about a command.

Options:
  --user=USERNAME  Use this user's vault

```

# Common settings paths

## GNOME settings
```
~/.config/dconf/user
```

## GNOME extensions
```
~/.local/share/gnome-shell/extensions
```

## APT sources
```
/etc/apt/sources.list
/etc/apt/sources.list.d
```

## Visual Studio Code settings
```
~/.config/Code/User/settings.json
```

# Quick install
```bash
sudo wget https://raw.githubusercontent.com/sbstp/vault/master/vault -O /usr/local/bin/vault && sudo chmod +x /usr/local/bin/vault
```
