## .envの設定

## 修正前
```bash
UID={UID}
GID={GID}
USER_NAME={swarmXX}
GROUP_NAME={swarmXX}
PASSWORD=swarm
HOMEWORKSPACE=argos_ws
```
## 修正手順
```bash
#UIDとGIDの変更
#ターミナルで実行
id

#例
root@Shota:~/argos_ws/docker-setup# id
uid=0(root) gid=0(root) groups=0(root),44(video),1000(docker)

#USER_NAMEとGROUP_NAMEの変更
#どちらもswarmXX
```
## X11サーバーにアクセス許可
```bash
#raspi5側で実行
xhost +local:docker
```