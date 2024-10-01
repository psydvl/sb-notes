#server #dnf


```bash
dnf -y install podman bash-completion vim pigz lsof fail2ban mosh
# dnf -y install epel-release
dnf install htop
systemctl enable fail2ban

```

```bash
transactional-update dup
transactional-update -c setup-selinux
transactional-update -c pkg install podman cockpit cockpit-tukit bash-completion fail2ban zstd rsync htop
systemctl enable fail2ban
cp /etc/fail2ban/jail.conf /etc/fail2ban/jail.local
vim /etc/fail2ban/jail.local # enable sshd here

```


## Backup
```template
[[Notes/Game/Rust#Backup]]
```


