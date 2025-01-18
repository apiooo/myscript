其它分流类型：
Clash 支持多种类型的规则，以下是常见的规则类型及其说明：

DOMAIN-SUFFIX：匹配指定域名后缀的流量。例如：
- DOMAIN-SUFFIX,example.com,Proxy
表示所有以 example.com 结尾的域名流量将通过 Proxy 代理。

DOMAIN-KEYWORD：匹配域名中包含指定关键字的流量。例如：
- DOMAIN-KEYWORD,keyword,Proxy
表示所有域名中包含 keyword 的流量将通过 Proxy 代理。

IP-CIDR：匹配指定 IP 段的流量。例如：
- IP-CIDR,192.168.0.0/16,Direct
表示 192.168.0.0/16 网段的流量将直接连接。

SRC-IP-CIDR：匹配指定源 IP 段的流量。例如：
- SRC-IP-CIDR,192.168.1.100/32,Proxy
表示源 IP 为 192.168.1.100 的流量将通过 Proxy 代理。

DST-PORT：匹配指定目标端口的流量。例如：
- DST-PORT,80,Direct
表示目标端口为 80 的流量将直接连接。

SRC-PORT：匹配指定源端口的流量。例如：
- SRC-PORT,1000,Proxy
表示源端口为 1000 的流量将通过 Proxy 代理。

GEOIP：匹配指定国家或地区的 IP 流量。例如：
- GEOIP,CN,Direct
表示中国的 IP 流量将直接连接。

GEOSITE：匹配指定类别的域名列表。例如：
- GEOSITE,category-ads,Reject
表示属于广告类别的域名流量将被拒绝。

IP-CIDR6：匹配指定 IPv6 段的流量。例如：
- IP-CIDR6,::1/128,Direct
表示 ::1/128 的 IPv6 流量将直接连接。

DOMAIN：匹配指定的完整域名。例如：
- DOMAIN,example.com,Proxy
表示 example.com 的流量将通过 Proxy 代理。
