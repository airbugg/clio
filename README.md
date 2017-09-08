# clio
Handy cli commands I use a lot

### Kill all `node` instances using `awk` (when `killall` just won't do)
```bash
❯ ps aux | awk '$11 ~ /node/ {print $2}' | xargs kill
```
