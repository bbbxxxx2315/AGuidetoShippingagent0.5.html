# 🚢 船代外勤 · 学习指南

> 为即将入职**船舶代理外勤岗位**的新人准备的全景式学习手册 - React 18 + Vite + TailwindCSS + Framer Motion + GSAP

[![React](https://img.shields.io/badge/React-18-61dafb)](https://react.dev)
[![Vite](https://img.shields.io/badge/Vite-5-646cff)](https://vitejs.dev)
[![TailwindCSS](https://img.shields.io/badge/TailwindCSS-3-38bdf8)](https://tailwindcss.com)
[![Framer Motion](https://img.shields.io/badge/Framer%20Motion-11-ff6e40)](https://www.framer.com/motion/)

## ✨ 项目亮点

- 🎨 **专业高级的视觉设计**：海洋蓝 + 暖橙双主题色系
- 🌀 **9 个关键动效**：滚动入场、悬停、飘动、菜单滑入、进度条、手写下划线、脉冲、旋转、招手
- 🧭 **6 大模块**：Header → Hero → 动效展示 → 三大分类 → 9 门课程 → 合作平台 → 邮件订阅 → Footer
- 📚 **9 门优质免费课程**：全部来自 985 高校和知名平台
- 📱 **完美响应式**：手机 / 平板 / 桌面自适应
- ⚡ **极速启动**：Vite + React 18 即时热更新

## 🚀 快速开始

```bash
# 1. 安装依赖
npm install

# 2. 启动开发服务器
npm run dev
# 浏览器自动打开 http://localhost:5173

# 3. 生产构建
npm run build

# 4. 预览生产构建
npm run preview
```

## 📁 项目结构

```
ship-agent-guide/
├── public/
│   └── anchor.svg              # 站点 favicon
├── src/
│   ├── components/
│   │   ├── Header.jsx          # 顶部导航（桌面 + 汉堡菜单）
│   │   ├── Hero.jsx            # 英雄区 + 统计数据
│   │   ├── Effects.jsx         # 9 个关键动效展示
│   │   ├── Categories.jsx      # 三大核心分类卡片
│   │   ├── Courses.jsx         # 9 门免费课程网格
│   │   ├── Partners.jsx        # 合作平台 Logo 墙
│   │   ├── Subscribe.jsx       # 邮件订阅表单
│   │   ├── Footer.jsx          # 页脚
│   │   ├── ScrollProgress.jsx  # 顶部滚动进度条
│   │   └── FloatingShapes.jsx  # 飘动装饰元素
│   ├── data/
│   │   └── content.js          # 课程、平台、分类等数据
│   ├── utils/
│   │   └── motionVariants.js   # Framer Motion 动画变体
│   ├── App.jsx                 # 主应用
│   ├── main.jsx                # 入口
│   └── index.css               # Tailwind + 全局样式
├── index.html
├── package.json
├── vite.config.js
├── tailwind.config.js          # 海洋蓝/暖橙双主题色
└── postcss.config.js
```

## 🎨 设计语言

### 配色
| 主题 | 用途 | 色值 |
|------|------|------|
| **Ocean 海洋蓝** | 主色 - 标题、背景、章节 | `#0c4a6e` → `#0ea5e9` |
| **Sunset 暖橙** | 强调色 - CTA、徽章、hover | `#f97316` → `#fed7aa` |
| **Sand 沙金** | 中性背景 | `#fdfcf7` → `#766838` |

### 字体
- **Nunito** - 圆润无衬线体（正文/标题）
- **Caveat** - 手写体（装饰性签名/小标签）

### 装饰元素
- ⚓ 锚、罗盘 🌊 浪、船 🚢 - 海洋主题图标
- 飘动圆点、虚线圆环 SVG
- 波浪分隔线（section 之间过渡）

## 🎬 9 个关键动效

| # | 动效 | 实现 |
|---|------|------|
| 01 | 滚动入场 | Framer Motion `whileInView` |
| 02 | 悬停放大 | Framer Motion `whileHover` + Spring |
| 03 | 飘动形状 | Tailwind `animate-float` keyframes |
| 04 | 菜单滑入 | Framer Motion `AnimatePresence` + x |
| 05 | 进度条 | Framer Motion `useScroll` + `useSpring` |
| 06 | 手绘下划线 | SVG `pathLength` 动画 |
| 07 | 脉冲呼吸 | Tailwind `animate-pulse-soft` |
| 08 | 旋转罗盘 | Tailwind `animate-spin-slow` |
| 09 | 摇摆招手 | Tailwind `animate-wave-hand` |

## 🛠 技术栈

- **React 18.3** - UI 框架
- **Vite 5** - 构建工具
- **TailwindCSS 3.4** - 原子化 CSS
- **Framer Motion 11** - 声明式动画
- **GSAP 3 + ScrollTrigger** - 滚动触发动画
- **Google Fonts** - Nunito + Caveat

## 📚 课程内容

所有课程均为**完全免费**，来自：

| 平台 | 课程 |
|------|------|
| 🎓 中国大学MOOC | 海商法、航运管理、航海英语、报关实务、国际货运代理 |
| 📚 超星学习通 | 国际船舶代理实务、国际航运管理、海关实务 |
| 🏛️ 学堂在线 | 海商法（清华平台） |
| 🌐 国家智慧教育 | 海商法、海运危险品运输 |

## 📱 响应式断点

```css
sm:  640px   /* 手机横屏 */
md:  768px   /* 平板 */
lg:  1024px  /* 桌面 */
xl:  1280px  /* 大屏 */
```

## 🤝 致谢

- 设计灵感来自 Squarespace 7.1 的高级单页式布局
- 配色与图标向海洋致敬
- 所有课程归原作者及平台所有

---

⚓ **愿你在港口的每一天，都与星辰大海为伴**
