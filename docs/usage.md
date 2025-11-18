---
title: 使用说明
sidebar: false
---

# 目录结构

```
docs/
  .vuepress/
    config.js
    styles/
  articles/
    java.md
    ...
  README.md
```

# 开发与发布

- 开发：`npm run docs:dev`
- 构建：`npm run docs:build`
- 预览：`npm run docs:preview`

# 新增文章

- 在 `docs/articles` 新建 `xxx.md`
- 在侧边栏中登记链接

# 样式定制

- 在 `docs/.vuepress/styles` 修改样式
- 保持无圆角、多线条与轻动效