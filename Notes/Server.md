#server #dnf


```bash
dnf -y install podman bash-completion vim pigz lsof fail2ban mosh
# dnf -y install epel-release
dnf install htop
systemctl enable fail2ban
```

## Backup

```bash
# backup
cd /
date >./server/time
tar -Ipigz -cf $(date -uI).server.$RANDOM.tar.gz ./server
cd /server/rust/data/server
1
# restore
cd /
tar -Ipigz -xf file.tar.gz
```