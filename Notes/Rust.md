#server #game #gameserver #rust

<https://gist.github.com/VaGo-o/5cfb21c03dc7e85f647a4eb6058aef79>

## Backup
```bash
# backup
cd /
tar -Ipigz -cf $(date -uI).server.$(($(date -u "+%s")%86400)).tar.gz ./server
cd /server/rust/data/server
tar -Ipigz -cf $(date -uI).server.only.$(($(date -u "+%s")%86400)).tar.gz ./rust

# restore
cd /
tar -Ipigz -xf file.tar.gz
```
