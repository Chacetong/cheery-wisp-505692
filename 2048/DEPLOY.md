# 🎮 2048 莫兰迪风格 - 部署指南

## 当前可玩链接

| 平台 | 链接 | 有效期 |
|------|------|--------|
| Cloudflare Tunnel | https://desert-afterwards-disturbed-migration.trycloudflare.com | 临时（服务器关闭后失效） |
| LocalTunnel | https://red-yaks-melt.loca.lt | 临时（服务器关闭后失效） |

## 永久部署方案

### 方案一：GitHub Pages（推荐）

1. **创建 GitHub 仓库**
   - 访问 https://github.com/new
   - 创建名为 `2048-game` 的公开仓库

2. **上传文件**
   ```bash
   git init
   git add index.html
   git commit -m "Initial commit"
   git branch -M main
   git remote add origin https://github.com/你的用户名/2048-game.git
   git push -u origin main
   ```

3. **开启 GitHub Pages**
   - 进入仓库 Settings → Pages
   - Source 选择 "Deploy from a branch"
   - Branch 选择 "main"，文件夹选择 "/ (root)"
   - 点击 Save

4. **访问游戏**
   - 链接格式：`https://你的用户名.github.io/2048-game`

### 方案二：Netlify Drop（最简单）

1. 访问 https://app.netlify.com/drop
2. 直接将 `index.html` 文件拖拽到页面上
3. 立即获得永久链接！

### 方案三：Vercel

1. 访问 https://vercel.com
2. 注册/登录账号（可用 GitHub 账号）
3. 创建新项目，导入或上传此项目
4. 自动部署，获得 `.vercel.app` 域名

### 方案四：Surge.sh

```bash
npm install -g surge
surge  # 按提示注册账号并部署
```

---

## 🎨 配色说明

采用**莫兰迪色系**设计：

| 数字 | 颜色 | 描述 |
|------|------|------|
| 2 | #e8e0d5 | 暖灰白 |
| 4 | #dcd4c8 | 浅驼色 |
| 8 | #c9b8a5 | 卡其色 |
| 16 | #b5a390 | 焦糖色 |
| 32 | #a69888 | 灰褐色 |
| 64 | #9a8b7a | 深驼色 |
| 128 | #8f9aa8 | 雾霾蓝 |
| 256 | #7a8a9a | 灰蓝色 |
| 512 | #6b7a8f | 深海蓝 |
| 1024 | #8fa68a | 灰豆绿 |
| 2048 | #7a8f75 | 苔藓绿 |

---

## 操作方式

- **桌面端**：方向键 ↑↓←→
- **移动端**：滑动屏幕或点击方向按钮
