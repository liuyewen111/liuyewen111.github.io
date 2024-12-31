Hi，大家好，我是 MH，今天的教程内容是在 Serv00 上安装 x-ui 面板并使用 ，让你的网速飞快 q (≧▽≦q)

如何安装 x-ui 面板？
申请端口
开启管理执行权限
执行一键脚本安装 x-ui 面板

步骤 1. 申请端口
登录你帐号对应的 panel 面板
面板左侧 > Port reservation > 选择 Add port 标签栏 > 勾选 Random > ＋Add
开放两个 TCP 端口，如 40402 和 40401（端口号可随便填写）
选择 Port list 标签栏 > 记录你分配到的 TCP 端口号
步骤 2. 开启管理执行权限
登录你帐号对应的 panel 面板
面板左侧 > 选择 Run your own applications 标签栏 > Enabled ; 使其 Status 变成 Enabled 即可
步骤 3. 执行一键脚本安装 x-ui 面板
`wget -O x-ui.sh -N --no-check-certificate https://raw.githubusercontent.com/amclubs/am-serv00-x-ui/main/x-ui.sh && chmod +x x-ui.sh && ./x-ui.sh `
注意：请确保 serv00 两个 TCP 端口开启

脚本会自动安装 x-ui 并配置环境
选择 1 安装 x-ui 面板
完成后，面板默认监听在 serv00 添加的第一个端口 40402（如果你是小白同学，中途让你做选择题时，你默认回车就🆗啦）
如何登陆 x-ui 面板？
添加域名
登录 x-ui 面板
步骤 1. 添加域名
登录你帐号对应的 panel 面板
面板左侧 > 选择 WWW.Websites 
复制 serv00 自带的域名如 athanaag.serv00.net，然后在删除（注意点中间的删除和软件）
标签栏 > Add New Websites
Domain 填入复制的域名名字 athanaag.serv00.net
点击 Advanced settings，将 Website type 中的 PHP 换成 Proxy
Proxy port 选择面板访问的端口 40402
然后点击 Add 进行添加
步骤 2. 登录 x-ui 面板
然后访问这个域名
输入默认用户名和密码：admin / admin（建议首次登录后立即更改密码）
如何配置节点？
创建节点
创建节点
进入 x-ui 面板后选择入站列表
点击 “+”
备注和端口填写在 serv00 添加的第二个端口 40401
传输选择 “ws”
最后点击添加就完成了
在详细信息中点击查看，再点击复制链接
将链接 Ctrl+V 复制到 V2rayN
总结
个人觉得还是使用甬哥的脚本才能让 serv00 发挥最大性能，虽说节点的速度一样，但甬哥的更有 Hysteria2 协议，且不用占用域名