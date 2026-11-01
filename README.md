# 26机智11班 班级小站

一个单文件的班级网站：通知、待办、树洞、日历、相册、私信、班宠乐园，全部数据存在云端（WorkBuddy 云服务 BaaS），页面本身无任何构建依赖。

## 部署

整个站就是一个 `index.html`，任何静态托管都能跑：

- **GitHub Pages**：仓库设置 → Pages → Source 选分支 / root，保存即可。
- 其它（Vercel / Netlify / 服务器）：把 `index.html` 当纯静态文件托管即可。

## 本地预览

直接双击 `index.html` 或：

```
python -m http.server 8080
# 打开 http://localhost:8080
```
