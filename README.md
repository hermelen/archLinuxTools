# rclone: Google Drive sync(especially)
https://rclone.org/docs/  
https://rclone.org/drive/  

### For Windows
Replace so user-friendly `rclone` with your rclone.exe location   
fe: `/c/rclone/rclone.exe copy GoogleDrive:keepass ~/Documents/Rclone/GoogleDrive/keepass`  
if rClone exe is located ther: `C:\rclone\rcloine.exe`

## List remotes
```console
rclone listremotes
```
returns
```console
GoogleDrive:
```

## Display one specific remote
```console
rclone lsd GoogleDrive:
```

`:` is important to specify that it is remote and not local

## Clone from remote:
```console 
rclone copy GoogleDrive:keepass ~/Documents/Rclone/GoogleDrive/keepass
```

## Push to remote
```console
rclone sync -i ~/Documents/Rclone/GoogleDrive/keepass GoogleDrive:keepass
```

