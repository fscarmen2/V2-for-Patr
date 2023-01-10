# V2ray for Patr

* * *

# 目录

- [项目特点](README.md#项目特点)
- [部署](README.md#部署)
- [免责声明](README.md#免责声明)

* * *

## 项目特点:
* 本项目用于在 Patr 免费服务上部署 V2ray ，采用的方案为 Nginx + WebSocket + VMess/VLess + TLS。DigitalOcean 新加坡的机器是免费的。
* V2ray 核心文件和配置文件作了“特殊处理”，每个项目都不同，大大降低被封和连坐风险
* vmess 和 vless 的 uuid，路径既可以自定义，又或者使用默认值
* 集成哪吒探针，可以自由选择是否安装
* 部署完成如发现不能上网，请检查域名是否被墙，可使用 Cloudflare CDN 或者 worker 解决。
* 部署时用到的镜像: `fscarmen/v2-koyeb` ， tag: `latest`

## 部署:
* 注册 [Patr.com](http://patr.cloud)
* 可用到的变量
  | 变量名 | 是否必须 | 默认值 | 备注 |
  | ------------ | ------ | ------ | ------ |
  | UUID         | 否 | de04add9-5c68-8bab-950c-08cd5320df18 | 可在线生成 https://www.zxgj.cn/g/uuid |
  | VMESS_WSPATH | 否 | /vmess | 以 / 开头 |
  | VLESS_WSPATH | 否 | /vless | 以 / 开头 |
  | NEZHA_SERVER | 否 |        | 哪吒探针服务端的 IP 或域名 |
  | NEZHA_PORT   | 否 |        | 哪吒探针服务端的端口 |
  | NEZHA_KEY    | 否 |        | 哪吒探针客户端专用 Key |

![image](https://user-images.githubusercontent.com/92626977/211455078-93d87631-e470-4583-a97a-fdd80b4ea0ec.png)
![image](https://user-images.githubusercontent.com/92626977/211455101-45a9e51d-c3fb-4ff4-b15f-fe5d679b9625.png)
![image](https://user-images.githubusercontent.com/92626977/211455115-337eccdc-ca7b-42c8-b5a4-ad5a823edbd7.png)
![image](https://user-images.githubusercontent.com/92626977/211455124-1e337eea-7491-40d5-8fd6-245e2c324422.png)
![image](https://user-images.githubusercontent.com/92626977/211455152-47630648-3891-4a8d-9f80-ce5749d86bb5.png)
![image](https://user-images.githubusercontent.com/92626977/211455163-0de63f86-4d33-4c49-aab3-e083d04e53c4.png)
![image](https://user-images.githubusercontent.com/92626977/211455170-4edec733-e646-49c5-9475-63f043a7fef6.png)
![image](https://user-images.githubusercontent.com/92626977/211455177-82b13a35-bac3-4c7c-ba39-71b7b412c282.png)
![image](https://user-images.githubusercontent.com/92626977/211455187-da0f7d38-6914-4f29-a6f0-d88d14e9c1be.png)

## 免责声明:
* 本程序仅供学习了解, 非盈利目的，请于下载后 24 小时内删除, 不得用作任何商业用途, 文字、数据及图片均有所属版权, 如转载须注明来源。
* 使用本程序必循遵守部署免责声明。使用本程序必循遵守部署服务器所在地、所在国家和用户所在国家的法律法规, 程序作者不对使用者任何不当行为负责。
