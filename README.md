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

# Quick install
```bash
sudo wget https://raw.githubusercontent.com/sbstp/vault/master/vault -O /usr/local/bin/vault && sudo chmod +x /usr/local/bin/vault
```
