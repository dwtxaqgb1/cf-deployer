# CF Worker 部署工具

基于 Cloudflare Workers API 的轻量级管理面板。支持多账号、在线编辑、一键部署、KV 管理、自定义域名绑定、备份回滚。

## 快速开始

    git clone https://github.com/dwtxaqgb1/cf-deployer.git
    cd cf-deployer/docker
    docker compose up -d --build

访问 `http://服务器IP:5100`

默认密码 `admin123`，**部署前请改 `docker/docker-compose.yml` 里的 `WEB_PASSWORD`**。

## 安全

- 默认密码 admin123，公开部署前必改
- 不要直接暴露公网，建议内网或加反代认证
- API Token 存在容器内 settings.json，注意不要提交
