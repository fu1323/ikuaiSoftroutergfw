# ikuaiSoftroutergfw
爱快透明代理 一个透明代理拓补图，跑在虚拟化平台，使用爱快软路由系统配合freebsd实现，借用ikuai内置多wan分流实现根据域名进行dns分流，
使用假wan环回流量从而突破ikuai分流器只能lan-wan分流的弊端，此方案下内网设备无需任何额外配置，不干扰bt下载 p2p连接，
缺点是必须禁用doH，必须把内网设备dns指向ikuai(如果部署了ADGuard 需将adguard上游dns只配置指向ikuai)必须手动维护域名列表（可以直接配置一级域名，常用大约300个），
对于需要ip直连的软件需要通过静态路由手动把地址段指向wan2(如Telegram)
![pdf.png](https://github.com/fu1323/ikuaiSoftroutergfw/blob/main/软路由拓补图.pnghttps://github.com/fu1323/ikuaiSoftroutergfw/blob/main/软路由拓补图.png)
