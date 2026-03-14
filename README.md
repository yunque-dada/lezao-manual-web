# 乐造内部培训手册

> 乐造AI员工内部培训话术手册网站

## 📋 项目概述

- **项目名称**：乐造内部培训手册
- **项目类型**：内部管理系统
- **核心功能**：提供员工话术培训、产品知识、课程顾问实战指南
- **目标用户**：乐造AI员工（课程顾问、前台等）

## 🛠 技术栈

| 技术 | 说明 |
|------|------|
| HTML5 | 页面结构 |
| CSS3 | 样式设计（原生CSS + 主题系统） |
| JavaScript | 交互逻辑、数据管理 |
| data.js | 动态数据（可后台编辑） |
| GitHub Pages | 部署托管 |

## 📁 目录结构

```
lezao-manual-web/
├── index.html          # 首页/课程列表
├── admin.html          # 后台管理（编辑data.js）
├── data.js             # 数据文件（课程、话术、问答）
├── styles.css         # 主样式
├── themes.css         # 主题系统
├── scratch.html       # Scratch课程
├── python.html        # Python课程
├── lego-duplo.html    # 乐高大颗粒
├── lego-wedo.html    # 乐高WeDo
├── data/              # 数据备份
└── README.md         # 开发文档
```

## 📄 页面功能

### 1. 首页 (index.html)
- 课程分类展示
- 快速搜索
- 主题切换（5套主题）

### 2. 课程页
- scratch.html：Scratch编程话术
- python.html：Python编程话术
- lego-duplo.html：乐高大颗粒课程
- lego-wedo.html：乐高WeDo机器人

### 3. 后台管理 (admin.html)
- 在线编辑data.js
- 预览效果
- 下载数据文件

## 💬 话术系统

### 每个课程包含
```javascript
{
  "speech": {
    "welcome": "开场白",
    "intro": "课程介绍",
    "objection": "处理异议"
  },
  "qa": [
    {"q": "常见问题", "a": "回答"}
  ]
}
```

## 🎨 主题系统

支持5套主题颜色（oklch）：

| 主题 | 主色 |
|------|------|
| orange（橙） | #f59e0b |
| blue（蓝） | #3b82f6 |
| green（绿） | #10b981 |
| purple（紫） | #8b5cf6 |
| rose（粉） | #f43f5e |

## 📊 数据结构 (data.js)

```javascript
var siteData = {
  "site": { title, orgName, contact, theme },
  "courses": {
    "scratch": { id, icon, title, subtitle, desc, prices, speech, qa },
    "python": { ... },
    "lego": { ... }
  }
}
```

## 🚀 部署

### GitHub Pages
```bash
cd lezao-manual-web
git add .
git commit -m "Add docs"
git push
```

## 📝 待完善

- [ ] 话术素材丰富
- [ ] 语音播报功能
- [ ] 考试测验模块

## 📊 更新日志

| 日期 | 内容 |
|------|------|
| 2026-03-10 | 创建项目，基础框架 |
| 2026-03-10 | 添加data.js数据系统 |
| 2026-03-10 | 完成5套主题系统 |
| 2026-03-10 | 后台admin.html支持编辑 |

## 🔗 相关链接

- 在线访问：https://yunque-dada.github.io/lezao-manual-web/
- GitHub：https://github.com/yunque-dada/lezao-manual-web

---
*最后更新：2026-03-14*
