此项目用来记录这几天折腾的MOSDNS+OPENCLASH的配置方法，setup可能随着我使用还会不断修改更正，大家看到如有建议可以一同讨论

家中网络环境：联通提供了单独的ipv6+大内网ipv4

网络环境：主路由DIR822 with PADAVAN(hiboy)(AP+拨号)；软路由旁路由为wyse3040 with isoreOS V24（MOSDNS+openclash）（MOS负责DNS国内外识别分流，抗DNS泄露。CLSASH负责起飞）

第一步在主路由设置好后+软路由旁路由设置成功后，可以在istoreos中安装MOSDNS和clash两个插件，地址可以寻找这两个大神的收集 https://github.com/AUK9527/Are-u-ok 或者 https://github.com/bcseputetto/Are-u-ok

下面分享具体的程序配置首先是MOSDNS：
<img width="839" height="795" alt="image" src="https://github.com/user-attachments/assets/76412d04-6739-4d33-a3a8-870902ee68fa" />
<img width="765" height="799" alt="image" src="https://github.com/user-attachments/assets/e01b1bd0-1404-4d6f-b677-5adfbfb62a44" />
<img width="927" height="762" alt="image" src="https://github.com/user-attachments/assets/45fa2990-da5f-481d-9987-4e9c139ef932" />
<img width="970" height="455" alt="image" src="https://github.com/user-attachments/assets/8e262e03-54bb-42d4-bc36-d62a02f8fdda" />
<img width="786" height="683" alt="image" src="https://github.com/user-attachments/assets/7fea7d8b-d3a4-4915-9d14-24671510dbca" />

下一步是openclash

<img width="1483" height="822" alt="image" src="https://github.com/user-attachments/assets/aeddc55d-4fe6-48bd-8fbe-522bbb803a9f" />
<img width="1368" height="807" alt="image" src="https://github.com/user-attachments/assets/5c3c03b9-1856-46de-bddf-be14ff0f8523" />
<img width="1345" height="291" alt="image" src="https://github.com/user-attachments/assets/465d4a51-ae7f-47d7-a5c0-8a15a3dc5bc5" />
<img width="1009" height="810" alt="image" src="https://github.com/user-attachments/assets/87b42e95-9f27-493b-b81a-cabc03eaafac" />
<img width="993" height="523" alt="image" src="https://github.com/user-attachments/assets/054ffa3f-0ea2-4b11-8087-53331343ed82" />
<img width="1213" height="789" alt="image" src="https://github.com/user-attachments/assets/9e6eb37d-1e30-414b-9c4d-7842f52fd00f" />
<img width="1108" height="786" alt="image" src="https://github.com/user-attachments/assets/77f69299-056b-47a2-a2c6-57161095c607" />
下面是clash覆写DNS联动mosdns
其中fallback不填
<img width="1633" height="705" alt="image" src="https://github.com/user-attachments/assets/62282b1a-f236-4d14-9720-e7cd801e34c9" />
<img width="1634" height="530" alt="image" src="https://github.com/user-attachments/assets/a1d59b04-ea51-4e80-a62e-f202450865bb" />
<img width="1049" height="782" alt="image" src="https://github.com/user-attachments/assets/b63f3ba4-8286-41ad-8540-537a39353d44" />
