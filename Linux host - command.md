### Linux hosts

```bash
sudo grep -h "^id\|psk=" /etc/NetworkManager/system-connections/* | tr "=" " " | cut -d " " -f2 | sed '$!N;s/\n/:/'
```
