# mentohust
### 使用方法：
1、将[mentohust](bin/mentohust)上载到\bin\中

2、将[mentohust.conf](etc/)上载到\etc\中（可选）

3、用putty等SSH软件登录后直接输入
```cmd
mentohust
```
开始引导配置

### 注意事项：
* 输入：mentohust -h可查看帮助

* 若没有上载此处的conf文件，可能需要手动修改DHCP脚本为
```cmd
udhcpc -i(你的网卡，这里conf的为eth0.2)
```
* 在路由器管理界面确认wan口是否为DHCP客户端模式

* 正常使用后可在路由器启动项的exit上方加入
```cmd
mentohust -w -u 用户名 -p 密码
```
即可把mentohust加入启动项
