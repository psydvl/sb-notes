#server #game #gameserver #rust

<https://gist.github.com/VaGo-o/5cfb21c03dc7e85f647a4eb6058aef79>

Dedicated server ID: 

## Backup
```rcon
save
writecfg
c.saveconfig
```

```bash
# backup
cd ~/
tar -I"zstd -6 -T0" -cf $(date -uI).$(($(date -u "+%s")%86400)).258550.full.tar.zst ./server
cd ~/server/rust/data/server
tar -I"zstd -6 -T0" -cf $(date -uI).$(($(date -u "+%s")%86400)).258550.only.rust.tar.zst ./rust

# restore
cd /
tar -Izstd -xf file.tar.gz

# rsync
rsync -havP host:/file.tar.gz ./
```
