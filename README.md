此项目用来记录这几天折腾的MOSDNS+OPENCLASH的配置方法，setup可能随着我使用还会不断修改更正，大家看到如有建议可以一同讨论
家中网络环境：联通提供了单独的ipv6+大内网ipv4
网络环境：主路由DIR822 with PADAVAN(hiboy)(AP+拨号)；软路由旁路由为wyse3040 with isoreOS V24（MOSDNS+openclash）（MOS负责DNS国内外识别分流，抗DNS泄露。CLSASH负责起飞）

第一步在主路由设置好后+软路由旁路由设置成功后，可以在istoreos中安装MOSDNS和clash两个插件，地址可以寻找这两个大神的收集 https://github.com/AUK9527/Are-u-ok 或者 https://github.com/bcseputetto/Are-u-ok

下面分享具体的程序配置首先是MOSDNS：
<img width="839" height="795" alt="image" src="https://github.com/user-attachments/assets/76412d04-6739-4d33-a3a8-870902ee68fa" />
<img width="765" height="799" alt="image" src="https://github.com/user-attachments/assets/e01b1bd0-1404-4d6f-b677-5adfbfb62a44" />
