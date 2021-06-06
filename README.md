## Homeland Docker

[Homeland](https://homeland.ruby-china.org/) 基于 Docker 的自动化部署方案。

## 系统需求

- Linux Server [4 Core CPU, 4G Memory, 50G Disk, 64 位] - _建议 Ubuntu Server 14.04_
- [Docker](https://www.docker.com/), [Docker Compose](https://docs.docker.com/compose/)
- [Aliyun OSS](https://www.aliyun.com/product/oss) 或 [UpYun](https://www.upyun.com) 用于文件存储。

## 使用说明

https://homeland.ruby-china.org/install/

## Versions

分支对应 Homeland 版本

- master - hoemland/homeland:3-8-latest
- 3-8-stable - hoemland/homeland:3-8-latest
- 3-7-stable - hoemland/homeland:3-7-latest
- 3-3-stable - hoemland/homeland:3-3-latest

## 部署管理工具

- 主要：make -> docker-compose -> docker
- 部分：make -> shell

## 主要组成部分

- homeland_app：应用服务 Puma
- homeland_app_backup：自动备份
- homeland_web：Web 服务 Nginx
- homeland_worker：延迟任务 Sidekiq
- homeland_caddy：自动 SSL 证书
- homeland_postgresql：数据库
- homeland_redis：缓存
