# JTA的业余无线电博客 MMDVM bi7jta.info  
 微信公众号 bi7jta73  
 QQ群 320533571 ; QQ微信在线 38091476  
 淘宝 [https://bi7jta.taobao.com](https://bi7jta.taobao.com)  
 视频 [https://space.bilibili.com/248541709](https://space.bilibili.com/248541709)     
 视频 [https://i.youku.com/bi7jta](https://i.youku.com/bi7jta)  
  
 教程 [PDF文件下载后浏览](https://github.com/huangqianqing/huangqianqing.github.io/tree/master/guide)   
 申请DMRID（必须将DMR设备登记到HAM执照）     
 自行提交 [https://www.radioid.net/register#!](https://www.radioid.net/register#!)     
 填表等待 [https://mmdvm.wufoo.com/forms/mmdvm-dmridaecee2/](https://mmdvm.wufoo.com/forms/mmdvm-dmridaecee2/)    
 
 DMR静态组设置（双工模式，双工板/中继板）  
 注册登录 [https://brandmeister.network/?page=rep-edit&id=460072323](https://brandmeister.network/?page=rep-edit&id=460072323)   
 
 在线线状态  
 通话记录  [https://hose.brandmeister.network/group/46001/](https://hose.brandmeister.network/group/46001/)  
 手机QSO  [Mumble/Pumble](https://github.com/huangqianqing/huangqianqing.github.io/tree/master/guide)  
 演示热点  [http://bi7jta.myq-see.com:8020/](http://bi7jta.myq-see.com:8020/)     
  
 MD380刷机   
 [教程图示](http://www.aprspi.org/mmdvm/md380-flash-firmware/)   
 [最新刷机包](https://github.com/huangqianqing/huangqianqing.github.io/tree/master/guide)  
 
   
更多：  
[www.aprspi.org](www.aprspi.org)   www.bi7jta.org  www.bi7jta.cn  www.mmdvm.io   

##新手必看  
准备局域网IP扫描APP：Fing ，各应用商店可以下载 [http://www.fing.com](http://www.fing.com)  
  
1，配置Wi-Fi，  
方法一，插网线，连接路由器，等待分配DHCP的IP地址，使用网页访问http://IP地址 ，进行配置，推荐先添加家庭Wi-Fi，重启。  
方法二，开机等待30秒到一分钟，热点会创建Wi-Fi管理AP节点，使用笔记本或者手机，搜索Wi-Fi网络Pi-Star，加入，打开浏览器访问 http://192.168.50.1，并在配置【Configuration】，滚动到最后，添加家庭Wi-Fi（推荐手工输入SSID/PSK），保存，断电重启。  
  
Wi-Fi的加入密码: raspberry  
网页访问用户/密码: pi-star/raspberry  
  
重启后，Wi-Fi路由器均会分配DHCP IP地址，使用局域网IP扫描APP，查找主机名为 Pi-Star的IP地址，使用http://IP地址 进入仪表盘。  
对于有屏幕的成品，OLED下屏幕在有有通联时，屏幕会显示IP地址；大屏幕连接正常时，待机界面底部会显示IP地址。  

2，配置Pi-Star，
对于成品，只需要修改你的DMRid/呼号即可，其它配置可使用默认值，DMR中国服务器 BM4601 
需要使用C4FM模式时，可以打开YSF模式开关，关闭DMR以防止多模式互联冲突。
YSF 中国组：YSF80337 - CN China 1 - W24166/TG46001
    
3，配置电台，  
YSF/C4FM:     
   设置呼号；单工板433.755MHz，双工模式TX434.755/RX439.755MHz，DN数字模式，无亚音；  
DMR:   
   设置DMRid，添加中国的通讯录「组呼46001」，接收组列表ALL包含「46001」，添加「信道CH46001」，发射联系人选择「46001」，接收组选择 「接收组ALL」，时隙2，彩色码1，功率低，频率同上。双工板/中继板可以开启双工模式，利用时隙1。  
  
4，调整误码率，  
http://pi-star/admin/expert/edit_mmdvmhost.php  
RXOffset   
TXOffset  
每次+-100，单位为Hz调整保存后按PTT观察仪表盘RF误码率，如果误码率<1%,在0.5%左右，属于正常范围，YSF会偏高点，也可以调到1%以内。  
  
5，更新DMRid数据，  
http://pi-star/admin/update.php  
  
*以上地址的【pi-star】不总是可以访问，推荐改成局域网DHCP分配的IP地址。  
 初次入门时，加QQ或微信:38091476 获得支持 ，深入学习交流加群   
  
 更多内容参考PDF文档。  