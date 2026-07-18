# Astrolabe · 星枢 隐私政策 (Privacy Policy)

中英双语隐私政策页面，可直接部署到 GitHub Pages。

**预览**：双击 `index.html` 在浏览器打开，左上角可切换中/英。

## 一键部署到 GitHub Pages（3 步）

### 1. 创建 GitHub 仓库

到 <https://github.com/new> 新建一个 **public** 仓库：

- 仓库名（建议）：`astrolabe-privacy`
- 描述：`Privacy Policy for Astrolabe · 星枢`
- 勾选 **Public**
- **不要**勾选 "Add a README" / "Add .gitignore"（保持空仓库）
- 点 **Create repository**

### 2. 推送文件

把整个 `astrolabe-privacy` 目录推上去：

```bash
cd /path/to/astrolabe-privacy
git init
git add .
git commit -m "Initial privacy policy"
git branch -M main
git remote add origin git@github.com:zhangfeiyang/astrolabe-privacy.git   # 替换成你的用户名
git push -u origin main
```

### 3. 开启 GitHub Pages

1. 打开仓库页面 → **Settings** → **Pages**
2. **Source** 选 `Deploy from a branch`
3. **Branch** 选 `main` / `(root)`
4. 点 **Save**

等 1-2 分钟后，访问：

```
https://zhangfeiyang.github.io/astrolabe-privacy/
```

这就是你的**隐私政策公开 URL**，复制下来填到 Google Play Console。

## 验证清单

部署完后：

- [ ] 用浏览器打开 URL，确认中英都能正常显示、切换
- [ ] 在 Chrome DevTools 的 "Lighthouse" 跑一遍无障碍检查
- [ ] 在 Google Play Console 的隐私政策 URL 字段填入这个 URL
- [ ] 用 <https://developers.google.com/search/docs/crawling-indexing/overview> 检查 Google 能不能抓取（可选但推荐）

## 文件结构

```
astrolabe-privacy/
├── index.html      # 单文件页面，含全部内容和样式
└── README.md       # 本说明
```

没有依赖、没有构建步骤，单文件即可运行。

## 修改日期

- 2026-07-18 — 首次发布
