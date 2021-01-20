<h1>winXray客户端使用</1>

<h3>winXray介绍:</h3>

winXray是Windows系统上简洁稳定的Xray/V2Ray、Shadowsocks、Trojan 通用客户端，可自动检测并连接访问速度最快的 代理服务器。
winXray可在服务器连接异常时自动更换代理服务器，再也不用担心服务器抽风了。使用感受上比qv2ray 2.7pre版相对稳定，至少无任何报错提示。

<h3>winXray优点:</h3>

1. 支持VMESS、VLESS、SS、trojan等多种协议；
2. 支持导入节点，使用方便；
3. 稳定；
4. 智能切换最快服务器。

<h3>winXray缺点:</h3>

1. 启动切换节点响应微慢；
2. 新增节点手动配置难度大；
3. 仅支持Windows平台，无法在Mac上使用。

<h3>winXray使用教程:</h3>

1. 从<a href="https://v2xtls.org/v2ray-windows%e5%ae%a2%e6%88%b7%e7%ab%af%e4%b8%8b%e8%bd%bd/">V2ray客户端</a>下载winXray；

2. winXray支持导入节点。如果你有节点URL或者订阅地址（支持V2ray/SS/Trojan，暂不支持Xray和XTLS），打开winXray客户端在“首页”列表中点右键，选择“自粘贴板批量导入分享链接和订阅源”，然后双击某个节点就可以使用了。
<img class="size-full wp-image-1469 lazyloaded" src="https://v2xtls.org/wp-content/uploads/2020/12/winXray客户端.jpg" data-src="https://v2xtls.org/wp-content/uploads/2020/12/winXray客户端.jpg" alt="winXray客户端" width="1030" height="690" data-srcset="https://v2xtls.org/wp-content/uploads/2020/12/winXray客户端.jpg 1030w, https://v2xtls.org/wp-content/uploads/2020/12/winXray客户端-300x201.jpg 300w, https://v2xtls.org/wp-content/uploads/2020/12/winXray客户端-1024x686.jpg 1024w, https://v2xtls.org/wp-content/uploads/2020/12/winXray客户端-768x514.jpg 768w" data-sizes="(max-width: 1030px) 100vw, 1030px" sizes="(max-width: 1030px) 100vw, 1030px" srcset="https://v2xtls.org/wp-content/uploads/2020/12/winXray客户端.jpg 1030w, https://v2xtls.org/wp-content/uploads/2020/12/winXray客户端-300x201.jpg 300w, https://v2xtls.org/wp-content/uploads/2020/12/winXray客户端-1024x686.jpg 1024w, https://v2xtls.org/wp-content/uploads/2020/12/winXray客户端-768x514.jpg 768w"><figcaption id="caption-attachment-1466" class="wp-caption-text">winXray客户端</figcaption>

3. winXray也支持手动配置节点，使用上相对较为麻烦。首先点击“配置”切换页面，然后以json方式手动填写节点信息。
<img class="size-full wp-image-1466 lazyloaded" src="https://v2xtls.org/wp-content/uploads/2020/12/winXray手动填写信息.jpg" data-src="https://v2xtls.org/wp-content/uploads/2020/12/winXray手动填写信息.jpg" alt="winXray手动填写信息" width="1031" height="692" data-srcset="https://v2xtls.org/wp-content/uploads/2020/12/winXray手动填写信息.jpg 1031w, https://v2xtls.org/wp-content/uploads/2020/12/winXray手动填写信息-300x201.jpg 300w, https://v2xtls.org/wp-content/uploads/2020/12/winXray手动填写信息-1024x687.jpg 1024w, https://v2xtls.org/wp-content/uploads/2020/12/winXray手动填写信息-768x515.jpg 768w" data-sizes="(max-width: 1031px) 100vw, 1031px" sizes="(max-width: 1031px) 100vw, 1031px" srcset="https://v2xtls.org/wp-content/uploads/2020/12/winXray手动填写信息.jpg 1031w, https://v2xtls.org/wp-content/uploads/2020/12/winXray手动填写信息-300x201.jpg 300w, https://v2xtls.org/wp-content/uploads/2020/12/winXray手动填写信息-1024x687.jpg 1024w, https://v2xtls.org/wp-content/uploads/2020/12/winXray手动填写信息-768x515.jpg 768w"><figcaption id="caption-attachment-1466" class="wp-caption-text">winXray手动填写信息</figcaption>

<h3>因手动配置节点较为麻烦，下面给出各种常用配置的模板：</h3>
<p><strong>VLESS+TCP+XTLS配置模板</strong></p>
<pre> {
        "address":"服务器ip或者域名",
        "flow":"xtls-rprx-direct",
        "id":"填写uuid",
        "network":"tcp",
        "port": 端口,
        "protocol":"vless",
        "ps":"填写备注",
        "tls":"xtls"
 }</pre>
