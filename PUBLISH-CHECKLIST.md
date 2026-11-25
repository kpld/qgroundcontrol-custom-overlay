# 发布清单（给 Li，发布前删掉本文件）

这个仓库骨架在我这边备好了，但有两样东西只有你 Windows 机器上有，
发布前需要你补进来：

1. **custom/ 真目录**：把 `D:\QtProjects\qgroundcontrol\custom\` 的内容
   拷到本仓库的 `custom/` 下（现在里面只有占位文件，拷完删掉
   `custom/PUT-CUSTOM-HERE.txt`）。注意别把 custom 里的 build 脏目录带进来。
2. **五航点截图**：存为 `docs/images/five-waypoint-mission.png`
   （README 顶部引用的就是这个文件名；就是你投 QGC 提案时留存的那张）。

发布步骤：
1. 在 GitHub 建空仓库 `qgroundcontrol-custom-overlay`（Public，不要勾选
   初始化 README）。
2. 加 deploy key 后 push（远程走 ssh.github.com:443 老通道）。
3. 推完检查主页 README 顶部截图正常显示、链接可点。
4. 然后再发主页 README 仓库（kpld/kpld），那边的链接就指向这个仓库。

隐私提醒：README 里 SITL 的 IP 用了占位符 `<sitl-host-ip>`，
没有写你家局域网的真实地址，不用改。
