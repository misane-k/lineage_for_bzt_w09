# 免责声明
刷机操作存在风险，可能导致设备损坏、数据丢失等不可预见情形，由此产生的一切后果均由您自行承担。本人对因您未正确理解或执行教程而引发的设备故障或其他损失，以及任何法律责任均不承担。对于教程中涉及的第三方软件、工具或资源，本人不对其安全性、合法性、有效性作任何担保。您应在充分知晓刷机风险与自身能力后，谨慎决定是否进行刷机操作。

# 使用方法
先[解bl锁](https://github.com/sora-orz/unflytek)，再刷入[底包](https://github.com/misane-k/lineage_for_bzt_w09/releases/download/v0/base.7z)，最后刷入LineageOS

# 修改
- 允许 ptrace，允许修改SELinux为 permissive
- 添加配置文件使5g wifi可用

# 已知问题
- 声卡，不连接蓝牙耳机时无声音

# 杂谈
所有CPU核心在启动时为EL1模式，而kvm需要EL2，所以kvm是**不可能**实现的。除非有工程机或者挖掘bootrom漏洞

# TODO
- 自定义机型、设备信息等
- 添加华为的MDM能力，这样就能正常使用并更新智慧课堂软件
- 有人需要的话，再把源码发出来吧，毕竟几乎没改

# 特别感谢
- [mashed-potatoes](https://github.com/mashed-potatoes/PotatoNV) 低版本海思芯片解bl锁方法
- [xtuiflyzhkt](https://github.com/xtuiflyzhkt/iflytek_cyzhkt_cr) C5解锁方法
- [氢氧化氢氢氢氢氢氢]([https://markdown.com.cn](https://space.bilibili.com/673804198)) 提供C5底包
- [huawei](https://download-c1.huawei.com/download/downloadCenter?downloadId=C0A375675F29E492D4DEDB28D30DB6B6) 内核源代码
- [LineageOS](https://github.com/LineageOS) [phhusson](https://github.com/phhusson/treble_experimentations) 让自定义安卓系统成为可能
