###  **git建库**
1. 直接在github中新建仓库
2. 在本地文件夹中用客户端`` git clone ``


### **git无法同步文件**
+ 反复测试代理问题

```// 查看当前代理设置
git config --global http.proxy
git config --global https.proxy
 
// 设置当前代理为 http://127.0.0.1:1080 或 socket5://127.0.0.1:1080
git config --global http.proxy 'http://127.0.0.1:1080'
git config --global https.proxy 'http://127.0.0.1:1080'
 
git config --global http.proxy 'socks5://127.0.0.1:1080'
git config --global https.proxy 'socks5://127.0.0.1:1080'
 
// 删除 proxy
git config --global --unset http.proxy
git config --global --unset https.proxy
```