# rclone: Google Drive sync(especially)
https://rclone.org/docs/  
https://rclone.org/drive/  
## List remotes
```console
rclone listremotes
```
returns
```console
GoogleDrive:
```

## Display on specific remote
```console
rclone lsd GoogleDrive:
```

`:` is important to specify that it is remote and not local

## Clone frome remote:
```console 
rclone copy GoogleDrive:keepass ~/Documents/Rclone/GoogleDrive/keepass
```

