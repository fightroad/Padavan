# padavan #

### 基于TSL大佬的padavan4.4版本。

- 默认信息如下
- ip：192.168.2.1
- 账号：admin
- 密码：admin
- wifi密码：1234567890

This project is based on original rt-n56u with latest mtk 4.4.198 kernel, which is fetch from D-LINK GPL code.

#### Extra functions / changes
- Adding user/chinadns-ng , and fix shadowsocks + chinadns-ng using local domain whitellist.
- AP Relay auto-daemon


#### SS/SSR
- Transparent proxy (iptables) wasn't cleaned completely, this issue is fixed.
- Adding DNSProxy , Local DNS integrated with SS/SSR 
- Dnsmasq optimization specially for SS/SSR 
- Resolve DNS pollution - Adding DNS i/p in china-route mode
- Fast-open option is enabled according to linux version
##### Enhancements in this repo

- commits has beed rewritten on top of [hanwckf/rt-n56u](https://github.com/hanwckf/rt-n56u) repo for better history tracking
- Optimized Makefiles and build scripts, added a toplevel Makefile
- Added ccache support, may save up to 50%+ build time
- Upgraded the toolchain and libc:
  - gcc 13.3.0
  - musl 1.2.5 / uClibc-ng 1.0.48
 - OpenWrt style package Makefile
 - Enabled kernel cgroups support
 - Fixed K2P led label names
 - Replaced udpxy with msd_lite
 - Replaced Web Console with ttyd
 - Upgraded libs and user packages
 - And a lot of package related fixes
 - ...

# Features

- Based on 4.4.198 Linux kernel
- Support MT7621 based devices
- Support MT7615D/MT7615N/MT7915D wireless chips
- Support raeth and mt7621 hwnat with legency driver
- Support qca shortcut-fe
- Support IPv6 NAT based on netfilter
- Support WireGuard integrated in kernel
- Support fullcone NAT (by Chion82)
- Support LED&GPIO control via sysfs

# Supported devices
- 360-T6M (from https://github.com/BINGHUAice/padavan-4.4, 没有机器测试，自行判断)
- B70
- BELL-A040WQ
- C-Life-XG1 (from https://github.com/vb1980/padavan-4.4, 没有机器测试，自行判断)
- CR660x
- DIR-878
- DIR-882
- EA7500 (from https://github.com/MNM28/padavan-4.4, 没有机器测试，自行判断)
- G-AX1800 (from https://github.com/ddyjyj/padavan-4.4, 富春江G-AX1800, 自测可用)
- G-AX1800-B (from https://github.com/vb1980/padavan-4.4, 富春江G-AX1800黑色版本，自测可用, 网口配置和白色版不一样，4根天线都是ipex可拆，ttl排针焊接好了，做工比白色版好些)
- GHL (from https://github.com/fangenhui520/padavan-4.4, 没有机器测试，自行判断)
- HAR-20S2U1 (from https://github.com/vb1980/padavan-4.4, 没有机器测试，自行判断)
- JDCloud RE-CP-02 (无线宝鲁班, from https://github.com/240038901/padavan-4.4, 没有机器测试，自行判断)
- JDCloud RE-SP-01B (from https://github.com/MeIsReallyBa/padavan-4.4, 没有机器测试，自行判断)
- JCG-836PRO
- JCG-AC860M
- JCQ-Q10Pro (from https://github.com/vb1980/padavan-4.4, 没有机器测试，自行判断)
- JCQ-Q11Pro (from https://github.com/qewwqewq22/padavan11, 没有机器测试，自行判断)
- JCG-Q20
- JCG-Y2
- K2P
- K2P-USB
- MI-4
- MI-R3G
- MI-R3P
- MI-R4A (from https://github.com/vipshmily/padavan-4.4, 自测可用)
- MR2600
- MSG1500
- MSG1500-Z (from https://github.com/TurBoTse/padavan, 自测可用)
- NETGEAR-BZV
- NETGEAR-R6800 (from https://github.com/MNM28/padavan-4.4, 没有机器测试，自行判断)
- NETGEAR-R7450 (from https://github.com/vipshmily/padavan-4.4, 自测可用)
- NEWIFI
- NEWIFI3 (partially from https://github.com/GH-X/padavan-4.4, 无需拆除C48电容，没有机器测试，自行判断)
- QM-B1 (from https://github.com/monw/padavan, 没有机器测试，自行判断)
- R2100
- RM2100
- RT-AC85P
- SIM-AX1800T (from https://github.com/vb1980/padavan-4.4, 没有机器测试，自行判断)
- TX1801 Plus (from https://github.com/MNM28/padavan-4.4, 没有机器测试，自行判断)
- WDR8620 (from https://github.com/fzn0268/padavan-4.4, 没有机器测试，自行判断)
- WE410443-TC (from https://github.com/akw28888/padavan-4.4, 没有机器测试，自行判断)
- WIA3300-10 (from https://github.com/vb1980/padavan-4.4, 西加云杉WIA3300-10，自测可用)
- WR1200JS
- XY-C1
