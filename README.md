# yhkc-apps

应用中心 - yhkc.club

## 项目结构

```
.
├── index.html                    # 首页（应用导航）
├── probability-explorer/         # 概率探索者游戏
│   └── index.html
└── vercel.json                   # Vercel 配置文件
```

## 部署步骤

### 1. 创建 GitHub 仓库

1. 登录 GitHub
2. 点击 "New repository"
3. 仓库名：`yhkc-apps`
4. 选择 "Public"（公开）
5. 点击 "Create repository"

### 2. 上传代码

**方法一：直接上传**
1. 在仓库页面点击 "uploading an existing file"
2. 拖拽本文件夹内所有文件到上传区域
3. 点击 "Commit changes"

**方法二：Git 命令**
```bash
git init
git add .
git commit -m "Initial commit"
git branch -M main
git remote add origin https://github.com/你的用户名/yhkc-apps.git
git push -u origin main
```

### 3. 部署到 Vercel

1. 登录 [vercel.com](https://vercel.com)（用 GitHub 账号登录）
2. 点击 "Add New Project"
3. 导入 `yhkc-apps` 仓库
4. 点击 "Deploy"
5. 等待部署完成，获得临时域名（如 `yhkc-apps.vercel.app`）

### 4. 绑定自定义域名

1. 在 Vercel 项目设置中找到 "Domains"
2. 添加域名：`yhkc.club`
3. 按提示在火山引擎添加 DNS 记录：
   - 类型：CNAME
   - 主机记录：@
   - 记录值：cname.vercel-dns.com
4. 等待 DNS 生效（通常几分钟到几小时）

### 5. 完成

访问 `https://yhkc.club` 即可看到应用中心！

## 添加新应用

1. 在项目根目录创建新文件夹（如 `app2/`）
2. 放入应用代码（index.html）
3. 在 `index.html` 首页添加应用卡片
4. 重新部署

## 联系方式

如有问题请联系开发者。