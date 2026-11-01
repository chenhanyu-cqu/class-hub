# 26机智11班 · 班级小站

同学访问的入口就是仓库首页 `index.html`：它是一个外壳页，全屏内嵌真正的班级小站
（WorkBuddy 云端托管），所以分享出去的链接是 `https://chenhanyu-cqu.github.io/class-hub/`，
看不到 workbuddy 字样。

- **外壳页**：根目录 `index.html`，只做全屏 iframe + 加载兜底，别改坏 sharecode 参数。
- **源码备份**：`source/index.html` 是小站完整源码（单文件，含全部前端逻辑）。
  改完源码后，需要在 WorkBuddy 里重新发布应用，外壳页不用动。

## 注意

- 云服务只认 WorkBuddy 分配的那个域名（精确 Origin 校验），所以页面必须以
  iframe 形式跑在外壳里、由云端域名执行，不能直接把源码当静态页发布。
- 如果哪天线上突然空白，先怀疑两点：① iframe 被上游加了 X-Frame-Options 限制；
  ② sharecode 变了。改外壳页里的 `src` 即可。
