# Quantumult X小白配置 制作 by Orz-3 TG频道：t.me/Orzmini 2023/02/19

[general]
server_check_url=http://cp.cloudflare.com/generate_204
dns_exclusion_list=*.cmpassport.com, *.jegotrip.com.cn, *.icitymobile.mobi, id6.me
geo_location_checker=http://ip-api.com/json/?lang=zh-CN, https://raw.githubusercontent.com/Orz-3/Orz-3/master/QuantumultX/IP.js
resource_parser_url=https://fastly.jsdelivr.net/gh/KOP-XIAO/QuantumultX@master/Scripts/resource-parser.js
excluded_routes=239.255.255.250/32
udp_whitelist=1-442, 444-65535

[dns]
no-ipv6
server=119.29.29.29
address=/mtalk.google.com/108.177.125.188
server=/dl.google.com/119.29.29.29
server=/dl.l.google.com/119.29.29.29
server=/update.googleapis.com/119.29.29.29
server=/*.dl.playstation.net/119.29.29.29
server=/amplifi.lan/system
server=/router.synology.com/system
server=/sila.razer.com/system
server=/router.asus.com/system
server=/routerlogin.net/system
server=/orbilogin.com/system
server=/www.LinksysSmartWiFi.com/system
server=/LinksysSmartWiFi.com/system
server=/myrouter.local/system
server=/www.miwifi.com/system
server=/miwifi.com/system
server=/mediarouter.home/system
server=/tplogin.cn/system
server=/tplinklogin.net/system
server=/melogin.cn/system
server=/falogin.cn/system

[policy]
static=全球加速, 香港节点, 台湾节点, 日本节点, 韩国节点, 狮城节点, 美国节点, 特殊节点, proxy, direct, img-url=https://raw.githubusercontent.com/Orz-3/mini/master/Color/Global.png
static=苹果服务, 香港节点, 台湾节点, 日本节点, 韩国节点, 狮城节点, 美国节点, 特殊节点, proxy, direct, img-url=https://raw.githubusercontent.com/Orz-3/mini/master/Color/Apple.png
static=港台番剧, 香港节点, 台湾节点, direct, img-url=https://raw.githubusercontent.com/Orz-3/mini/master/Color/StreamingSE.png
static=国际媒体, 香港节点, 台湾节点, 日本节点, 韩国节点, 狮城节点, 美国节点, 特殊节点, proxy, img-url=https://raw.githubusercontent.com/Orz-3/mini/master/Color/Streaming.png
static=电报代理, 狮城节点, proxy, direct, img-url=https://raw.githubusercontent.com/Orz-3/mini/master/Color/Telegram.png
static=黑白名单, 香港节点, 台湾节点, 日本节点, 韩国节点, 狮城节点, 美国节点, 特殊节点, proxy, direct, img-url=https://raw.githubusercontent.com/Orz-3/mini/master/Color/Final.png
static=特殊节点, server-tag-regex=^(?!.*(港|台|日|韩|坡|美|HK|US|TW|JP|KR|SG|Hong|Tai|Japan|Korea|Singapore|States)), img-url=https://raw.githubusercontent.com/Orz-3/mini/master/Color/Static.png
url-latency-benchmark=香港节点, server-tag-regex=(?=.*(港|HK|(?i)Hong))^((?!(台|日|韩|新|美)).)*$, check-interval=600, tolerance=0, img-url=https://raw.githubusercontent.com/Orz-3/mini/master/Color/HK.png
url-latency-benchmark=台湾节点, server-tag-regex=(?=.*(台|TW|(?i)Taiwan))^((?!(港|日|韩|新|美)).)*$, check-interval=600, tolerance=0, img-url=https://raw.githubusercontent.com/Orz-3/mini/master/Color/TW.png
url-latency-benchmark=日本节点, server-tag-regex=(?=.*(日|JP|(?i)Japan))^((?!(港|台|韩|新|美)).)*$, check-interval=600, tolerance=0, img-url=https://raw.githubusercontent.com/Orz-3/mini/master/Color/JP.png
url-latency-benchmark=韩国节点, server-tag-regex=(?=.*(韩|韓|朝|KR|(?i)Korea))^((?!(港|台|日|新|美)).)*$, check-interval=600, tolerance=0, img-url=https://raw.githubusercontent.com/Orz-3/mini/master/Color/KR.png
url-latency-benchmark=狮城节点, server-tag-regex=(?=.*(新|狮|獅|SG|(?i)Singapore))^((?!(港|台|日|韩|兰|美)).)*$, check-interval=600, tolerance=0, alive-checking=false, img-url=https://raw.githubusercontent.com/Orz-3/mini/master/Color/SG.png
url-latency-benchmark=美国节点, server-tag-regex=(?=.*(美|US|(?i)States|American))^((?!(港|台|日|韩|新)).)*$, check-interval=600, tolerance=0, img-url=https://raw.githubusercontent.com/Orz-3/mini/master/Color/US.png

[server_remote]

[filter_remote]
https://raw.githubusercontent.com/DivineEngine/Profiles/master/Surge/Ruleset/Unbreak.list, tag=规则修正, force-policy=direct, update-interval=172800, opt-parser=true, enabled=true
https://raw.githubusercontent.com/DivineEngine/Profiles/master/Surge/Ruleset/Guard/Advertising.list, tag=广告拦截, force-policy=reject, update-interval=172800, opt-parser=true, enabled=true
https://raw.githubusercontent.com/DivineEngine/Profiles/master/Surge/Ruleset/Guard/AdvertisingPlus.list#type=domain-set, tag=广告拦截, force-policy=reject, update-interval=172800, opt-parser=true, enabled=true
https://raw.githubusercontent.com/NobyDa/Script/master/Surge/AdRule.list, tag=广告拦截, force-policy=reject, update-interval=172800, opt-parser=true, enabled=true
https://raw.githubusercontent.com/app2smile/rules/master/rule/tieba-ad-qx.list, tag=贴吧广告, force-policy=reject, update-interval=172800, opt-parser=false, enabled=true
https://raw.githubusercontent.com/DivineEngine/Profiles/master/Surge/Ruleset/Guard/Hijacking.list, tag=运营劫持, force-policy=reject, update-interval=172800, opt-parser=true, enabled=true
https://raw.githubusercontent.com/DivineEngine/Profiles/master/Surge/Ruleset/Guard/Privacy.list, tag=隐私保护, force-policy=reject, update-interval=172800, opt-parser=true, enabled=true
https://raw.githubusercontent.com/DivineEngine/Profiles/master/Surge/Ruleset/StreamingMedia/Video/TikTok.list, tag=海外抖音, force-policy=全球加速, update-interval=172800, opt-parser=true, enabled=true
https://raw.githubusercontent.com/DivineEngine/Profiles/master/Surge/Ruleset/Extra/Google/GoogleVoice.list, tag=Google Voice, force-policy=美国节点, update-interval=172800, opt-parser=true, enabled=true
https://raw.githubusercontent.com/DivineEngine/Profiles/master/Surge/Ruleset/Extra/Telegram/Telegram.list, tag=电报代理, force-policy=电报代理, update-interval=172800, opt-parser=true, enabled=true
https://raw.githubusercontent.com/DivineEngine/Profiles/master/Surge/Ruleset/StreamingMedia/Region/HK.list, tag=流媒体HK, force-policy=香港节点, update-interval=172800, opt-parser=true, enabled=true
https://raw.githubusercontent.com/DivineEngine/Profiles/master/Surge/Ruleset/StreamingMedia/Region/TW.list, tag=流媒体TW, force-policy=台湾节点, update-interval=172800, opt-parser=true, enabled=true
https://raw.githubusercontent.com/DivineEngine/Profiles/master/Surge/Ruleset/StreamingMedia/Region/JP.list, tag=流媒体JP, force-policy=日本节点, update-interval=172800, opt-parser=true, enabled=true
https://raw.githubusercontent.com/DivineEngine/Profiles/master/Surge/Ruleset/StreamingMedia/Region/US.list, tag=流媒体US, force-policy=美国节点, update-interval=172800, opt-parser=true, enabled=true
https://raw.githubusercontent.com/DivineEngine/Profiles/master/Surge/Ruleset/StreamingMedia/Streaming.list, tag=国际媒体, force-policy=国际媒体, update-interval=172800, opt-parser=true, enabled=true
https://raw.githubusercontent.com/DivineEngine/Profiles/master/Surge/Ruleset/StreamingMedia/StreamingSE.list, tag=港台番剧, force-policy=港台番剧, update-interval=172800, opt-parser=true, enabled=true
https://raw.githubusercontent.com/DivineEngine/Profiles/master/Surge/Ruleset/Global.list, tag=全球加速, force-policy=全球加速, update-interval=172800, opt-parser=true, enabled=true
https://raw.githubusercontent.com/DivineEngine/Profiles/master/Surge/Ruleset/Extra/Apple/Apple.list, tag=苹果服务, force-policy=苹果服务, update-interval=172800, opt-parser=true, enabled=true
https://raw.githubusercontent.com/DivineEngine/Profiles/master/Surge/Ruleset/China.list, tag=国内网站, force-policy=direct, update-interval=172800, opt-parser=true, enabled=true

[rewrite_remote]
https://raw.githubusercontent.com/Peng-YM/Sub-Store/master/config/QX.snippet, tag=Sub Store, update-interval=172800, opt-parser=false, enabled=true
https://raw.githubusercontent.com/chavyleung/scripts/master/box/rewrite/boxjs.rewrite.quanx.conf, tag=BoxJs, update-interval=172800, opt-parser=false, enabled=true
https://raw.githubusercontent.com/Orz-3/QuantumultX/master/Bili_Auto_Regions.conf, tag=Bilibili换区脚本, update-interval=172800, opt-parser=false, enabled=false
https://raw.githubusercontent.com/Orz-3/QuantumultX/master/JD_TB_price.conf, tag=比价脚本, update-interval=172800, opt-parser=false, enabled=false
https://raw.githubusercontent.com/NobyDa/Script/master/QuantumultX/TestFlightDownload.conf , tag=TestFlight区域限制解除, update-interval=172800, opt-parser=false, enabled=true
https://raw.githubusercontent.com/Orz-3/QuantumultX/master/TikTok.conf, tag=Tiktok解锁, update-interval=172800, opt-parser=false, enabled=true
https://raw.githubusercontent.com/Orz-3/QuantumultX/master/Netflix_ratings.conf, tag=Netflix评分, update-interval=172800, opt-parser=false, enabled=true
https://raw.githubusercontent.com/DivineEngine/Profiles/master/Quantumult/Rewrite/General.conf, tag=神机重定向, update-interval=172800, opt-parser=false, enabled=true
https://raw.githubusercontent.com/DivineEngine/Profiles/master/Quantumult/Rewrite/Block/YouTubeAds.conf, tag=YouTube去广告, update-interval=172800, opt-parser=false, enabled=false
https://raw.githubusercontent.com/app2smile/rules/master/module/bilibili-qx.conf, tag=Bilibili去广告, update-interval=172800, opt-parser=false, enabled=false
https://raw.githubusercontent.com/app2smile/rules/master/module/tieba-qx.conf, tag=贴吧去广告, update-interval=172800, opt-parser=false, enabled=false
https://raw.githubusercontent.com/DivineEngine/Profiles/master/Quantumult/Rewrite/Block/Advertising.conf, tag=神机去广告, update-interval=172800, opt-parser=true, enabled=true
https://raw.githubusercontent.com/NobyDa/Script/master/QuantumultX/Rewrite_lhie1.conf, tag=lhie1去广告, update-interval=172800, opt-parser=false, enabled=false
https://raw.githubusercontent.com/fmz200/wool_scripts/main/QuantumultX/rewrite/chongxie.txt, tag=张军去广告, update-interval=172800, opt-parser=false, enabled=false
https://raw.githubusercontent.com/DivineEngine/Profiles/master/Quantumult/Rewrite/Block/AdvertisingPlus.conf, tag=去广告脚本, update-interval=172800, opt-parser=false, enabled=true

[server_local]

[filter_local]
host-suffix, local, direct
ip-cidr, 192.168.0.0/16, direct
ip-cidr, 10.0.0.0/8, direct
ip-cidr, 172.16.0.0/12, direct
ip-cidr, 127.0.0.0/8, direct
ip-cidr, 100.64.0.0/10, direct
ip-cidr, 224.0.0.0/4, direct
ip6-cidr, fe80::/10, direct
ip-cidr, 203.107.1.1/24, reject
ip-cidr, 183.240.197.130/32, direct
final, 黑白名单

[rewrite_local]

[task_local]
event-interaction https://raw.githubusercontent.com/KOP-XIAO/QuantumultX/master/Scripts/streaming-ui-check.js, tag=流媒体解锁查询, img-url=arrowtriangle.right.square.system, enabled=true

[http_backend]

[mitm]
skip_validating_cert = true