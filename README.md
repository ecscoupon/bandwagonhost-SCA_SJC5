# 搬瓦工圣何塞USCA_SJC5机房VPS测评｜三网CN2 GIA精品回程，硬件质量、网络延迟、解锁流媒体深度实测

搬瓦工（BandwagonHost）提供美国圣何塞（USCA_SJC5）机房VPS，走的是优化线路，即三网回程CN2 GIA，平均ping延迟低于160ms，比较适合建站、中转等使用场景。

接下来将通过常见Linux命令对搬瓦工圣何塞机器进行测评，包括硬件质量、带宽速度、路由延迟、网络质量、IP质量等几个方面，所以测评数据仅供参考，具体请以实际使用为准。

## 关于搬瓦工BandwagonHost

搬瓦工是加拿大 IT7 旗下的海外主机商，其VPS采用 KVM 虚拟化、Raid10 SSD，带宽 1Gbps 起。机房覆盖洛杉矶、香港、日本、荷兰等，支持 KiwiVM 面板一键切换机房，有 CN2 GT、CN2 GIA等多种优化线路。优势是线路选择丰富、稳定性好、速度快，面板功能齐全；缺点是工单响应偏慢，优质CN2 GIA套餐价格偏高。

**<a href="https://bwh89.net/aff.php?aff=71768" target="_blank" rel="nofollow noopener noreferrer">搬瓦工官网：点此直达</a>**

<img width="688" height="536" src="https://github.com/ecscoupon/pictures/blob/main/bww.png" alt="搬瓦工官网">

##  测试机器方案配置 

本次记录的套餐为 SPECIAL 20G KVM PROMO V5 - CN2 GIA ECOMMERCE ，参数配置如下：

SSD: 20 GB RAID-10

RAM: 1GB

CPU: 2x Intel Xeon

Transfer: 1000 GB/mo

Link speed: 2.5 Gigabit

搬瓦工美国圣何塞（USCA_SJC5）基于KVM虚拟化，宿主机为Intel Sierra Forest，RAID-10 SSD阵列，最高10Gbps带宽，自带快照和备份功能，自带1个IPv4和IPv6，支持常见Linux发行版，$49.99/季起：
<ul>
 	<li><span style="color: #ff9900;">记得选择“US - San Jose (USCA_SJC5)”机房</span></li>
 	<li><span style="color: #ff9900;">该系列可以在16个机房之间一键切换（不包括日本、新加坡、香港CN2 GIA）</span></li>
</ul>
<table>
<tbody>
<tr>
<td style="text-align: center;"><strong>内存</strong></td>
<td style="text-align: center;"><strong>CPU</strong></td>
<td style="text-align: center;"><strong>硬盘</strong></td>
<td style="text-align: center;"><strong>流量</strong></td>
<td style="text-align: center;"><strong>带宽</strong></td>
<td style="text-align: center;"><strong>租用价格</strong></td>
<td style="text-align: center;"><strong>购买地址</strong></td>
</tr>
<tr>
<td style="text-align: center;">1GB</td>
<td style="text-align: center;">2核</td>
<td style="text-align: center;">20GB SSD</td>
<td style="text-align: center;">1TB/月</td>
<td style="text-align: center;">2.5Gbps</td>
<td style="text-align: center;"><span style="color: #ff0000;">49.99美元/季</span></td>
<td style="text-align: center;"><a href="https://bwh89.net/aff.php?aff=71768&pid=87" target="_blank" rel="noopener">官网购买</a></td>
</tr>
<tr>
<td style="text-align: center;">2GB</td>
<td style="text-align: center;">3核</td>
<td style="text-align: center;">40GB SSD</td>
<td style="text-align: center;">2TB/月</td>
<td style="text-align: center;">2.5Gbps</td>
<td style="text-align: center;"><span style="color: #ff0000;">89.99美元/季</span></td>
<td style="text-align: center;"><a href="https://bwh89.net/aff.php?aff=71768&pid=88" target="_blank" rel="noopener">官网购买</a></td>
</tr>
<tr>
<td style="text-align: center;">4GB</td>
<td style="text-align: center;">4核</td>
<td style="text-align: center;">80GB SSD</td>
<td style="text-align: center;">3TB/月</td>
<td style="text-align: center;">2.5Gbps</td>
<td style="text-align: center;"><span style="color: #ff0000;">56.99美元/月</span></td>
<td style="text-align: center;"><a href="https://bwh89.net/aff.php?aff=71768&pid=89" target="_blank" rel="noopener">官网购买</a></td>
</tr>
<tr>
<td style="text-align: center;">8GB</td>
<td style="text-align: center;">6核</td>
<td style="text-align: center;">160GB SSD</td>
<td style="text-align: center;">5TB/月</td>
<td style="text-align: center;">5Gbps</td>
<td style="text-align: center;"><span style="color: #ff0000;">86.99美元/月</span></td>
<td style="text-align: center;"><a href="https://bwh89.net/aff.php?aff=71768&pid=90" target="_blank" rel="noopener">官网购买</a></td>
</tr>
<tr>
<td style="text-align: center;">16GB</td>
<td style="text-align: center;">8核</td>
<td style="text-align: center;">320GB SSD</td>
<td style="text-align: center;">8TB/月</td>
<td style="text-align: center;">5Gbps</td>
<td style="text-align: center;"><span style="color: #ff0000;">159.99美元/月</span></td>
<td style="text-align: center;"><a href="https://bwh89.net/aff.php?aff=71768&pid=91" target="_blank" rel="noopener">官网购买</a></td>
</tr>
<tr>
<td style="text-align: center;">32GB</td>
<td style="text-align: center;">10核</td>
<td style="text-align: center;">640GB SSD</td>
<td style="text-align: center;">10TB/月</td>
<td style="text-align: center;">10Gbps</td>
<td style="text-align: center;"><span style="color: #ff0000;">289.99美元/月</span></td>
<td style="text-align: center;"><a href="https://bwh89.net/aff.php?aff=71768&pid=92" target="_blank" rel="noopener">官网购买</a></td>
</tr>
<tr>
<td style="text-align: center;">64GB</td>
<td style="text-align: center;">12核</td>
<td style="text-align: center;">1280GB SSD</td>
<td style="text-align: center;">12TB/月</td>
<td style="text-align: center;">10Gbps</td>
<td style="text-align: center;"><span style="color: #ff0000;">549.99美元/月</span></td>
<td style="text-align: center;"><a href="https://bwh89.net/aff.php?aff=71768&pid=93" target="_blank" rel="noopener">官网购买</a></td>
</tr>
</tbody>
</table>
<ul>
 	<li>默认支持1个IPv4和IPv6</li>
 	<li>自带免费备份+免费快照</li>
</ul>

### 综合测评数据分享如下

**硬件质量检测报告：** Geekbench 单核 835、多核 1607，CPU 性能属于入门水平。内存 1G，支持 KSM 复用。 磁盘FIO测试：随机 4K 读写约 23~27MB/s，顺序读写可达 1.6GB/s 左右，小文件随机性能一般，大文件吞吐尚可。 整机HQ硬件加权总分30603，适合轻量型等低负载业务，不适合数据库等高IO、高算力场景。

<img src="https://github.com/ecscoupon/pictures/blob/main/bwgshjceping.png" alt="硬件质量检测报告">

**IPv4大包回程路由测试：** 电信全国各地区延迟稳定在 180ms以下，全程 0 丢包。 联通大部分地区 CN2 GIA 直连，延迟 144 ~ 200ms，仅少数省份出现 163 转 4837 跳转，贵州存在 18% 丢包，北京 8% 丢包。 移动同样 CN2 GIA 回程，延迟 133 ~ 222ms，部分省份有少量丢包（最高 16%）。 整体基线很不错，大部分省份低延迟零丢包，仅个别地区有轻微丢包。

<img src="https://github.com/ecscoupon/pictures/blob/main/bwgshjcepin.png" alt="IPv4大包回程路由测试">

教育网回程路由延迟测试结果：

<img src="https://github.com/ecscoupon/pictures/blob/main/bwgshjcepi.png" alt="教育网回程路由延迟测试结果">

三网部分节点延迟测试数据：

<img src="https://github.com/ecscoupon/pictures/blob/main/bw.png" alt="三网部分节点延迟测试数据">

**国际节点TCP互联网络测试结果：**  IPv4：全球大部分节点延迟良好且零丢包。亚洲日本延迟较低；美洲、欧洲各大节点延迟低，仅巴西里约热内卢上传出现严重重传。 IPv6：美、欧、大洋洲整体稳定无丢包；但香港、新加坡节点存在上传重传问题。 

<img src="https://github.com/ecscoupon/pictures/blob/main/bwgshjcep.png" alt="国际节点TCP互联网络测试">

**单线程上行和下行带宽速度测试：** TCP 采用 BBR 拥塞控制，fq 排队算法。 电信、联通单线程上下行速度很强，回程可达 500~670Mbps，延迟稳定，丢包为 0；移动明显短板，上下行速度大幅缩水，存在少量重传。 国际方向 Apple 节点带宽拉满，IPv4 下载接近 5.5Gbps，上传 2.2Gbps，零丢包。

<img src="https://github.com/ecscoupon/pictures/blob/main/bwgshjce.png" alt="单线程上行和下行带宽速度测试">

回程路由节点详细测试结果：

<img src="https://github.com/ecscoupon/pictures/blob/main/bwgshjc.png" alt="回程路由节点">

**IPv4网络质量体检报告：** 三网回程均为 CN2线路，国内电信、联通延迟稳定，移动延迟略高。 国内测速节点部分测试失败；国际互联表现优秀，美西节点延迟极低，香港、新加坡、欧洲节点延迟可控，仅少数节点测试报错。 上游非 Tier1，整体网络质量较强。

<img src="https://github.com/ecscoupon/pictures/blob/main/bwgshj.png" alt="IPv4网络质量体检报告">

IPv6网络质量检测报告：

<img src="https://github.com/ecscoupon/pictures/blob/main/bwgsh.png" alt="IPv6网络质量检测报告">

**IPv4质量检测数据报告：** 属于机房广播 IP。风险整体偏低，多个库标记为机房商业 IP。 TikTok、Disney+、Netflix、AmazonPV、Reddit、ChatGPT全部原生解锁。25 端口出站可用，主流邮箱连通正常，IP黑名单数量为 0。

<img src="https://github.com/ecscoupon/pictures/blob/main/bwgs.png" alt="IPv4质量检测数据报告">

IPv6质量检测数据报告：

<img src="https://github.com/ecscoupon/pictures/blob/main/bwg.png" alt="IPv6质量检测数据报告">

## 本次测评小结 - 仅供参考

这台搬瓦工圣何塞 KVM 小鸡，配置是 2 核 2 线程、1G 内存、19G 硬盘，跑 Debian12差异，BBR+fq 算法就位。CPU 属于入门水平，跑轻量任务够用；硬盘小文件随机性能一般，但大文件顺序读写很强。

网络方面，三网回程全是CN2线路！国内电信、联通延迟低且基本零丢包，移动延迟略高，单线程测速电信联通能跑到 500Mbps 以上，唯独移动带宽拉胯。国际出口实力强悍，访问美西延迟极低，日韩、欧洲节点表现稳定，仅少数远距离节点偶有重传。另外，IP 是机房广播 IP，整体风险低。流媒体解锁直接拉满，TikTok、奈飞、ChatGPT 等全部原生解锁。

总的来说，适合建站业务。短板也是有的，例如算力偏弱，移动线路限速严重，有机房IP标签，不适合跑高负载数据库和对移动大流量有需求的业务。
