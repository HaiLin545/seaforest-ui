# 🌊🌲 SeaForest Design System

> *"Where the ocean breathes through the pines."*
> 海松青、晨雾蓝、珊瑚橙——一套为现代 Web、App、桌面端打造的、有呼吸感的设计系统。

SeaForest 的灵感来自**清晨海岸边的松林**：海雾带着微咸，阳光透过针叶洒下青绿与金色的光斑。它融合了**海洋的开阔**与**森林的静谧**，既**简约大气**，又**活泼现代**。

面向喜欢前端、Web3D、图形学、游戏的创作者，SeaForest 希望在界面中留下"光"与"水"的质感。

---

## 1. 设计哲学（Design Philosophy）

四个关键词概括 SeaForest 的性格：

### 🌊 Fluid · 流
像水与雾一样柔软。渐变、模糊、光晕是主角；硬边框与分割线被尽可能弱化。

### 🌲 Grounded · 定
海再开阔，也有礁石与岛屿。清晰的层级、可预期的栅格、稳定的节奏，让用户始终知道自己在哪儿。

### 💡 Luminous · 光
SeaForest 善用**微光**——玻璃拟态、柔和高光、极光渐变，让界面看起来"自带光源"，现代而有温度。

### ⚡ Precise · 精
每一处对齐、每一条曲线、每一次过渡都经过打磨。向工程师的精度偏好致敬。

---

## 2. 色彩系统（Color System）

SeaForest 放弃了传统老气的森林绿，采用**海松青（Teal）** 作为主品牌色——它既是森林的绿，也是海洋的蓝，现代、年轻、不容易审美疲劳。

### 2.1 原色板（Core Palette）

#### 🌊 Seafoam Teal（主品牌色 · 海松青）
带蓝调的青绿，像浅海倒映松林。

| Token | HEX | 用途 |
|-------|-----|------|
| `teal-50`  | `#ECFBF7` | 最浅背景 |
| `teal-100` | `#CFF4EA` | 浅填充 |
| `teal-200` | `#9FE6D4` | 次级填充 |
| `teal-300` | `#5FD1B8` | 辅助强调 |
| `teal-400` | `#22B89A` | 次级品牌 |
| `teal-500` | `#0E9F86` | **主品牌色 / Primary** |
| `teal-600` | `#0A806C` | Hover |
| `teal-700` | `#086654` | Active |
| `teal-800` | `#074D40` | 深色装饰 |
| `teal-900` | `#053830` | 深色背景辅助 |

#### 🌌 Deep Sea Blue（二级主题色 · 深海蓝）
低饱和的深海蓝，与 Teal 搭配形成"浅海 × 深海"的层次。

| Token | HEX | 用途 |
|-------|-----|------|
| `sea-50`  | `#EEF4FB` |
| `sea-100` | `#D5E4F4` |
| `sea-200` | `#A6C3E4` |
| `sea-300` | `#6D9BCF` |
| `sea-400` | `#427BB9` |
| `sea-500` | `#2C5E96` | 次要品牌 / Info |
| `sea-600` | `#234B78` |
| `sea-700` | `#1B3B5E` |
| `sea-800` | `#142B45` |
| `sea-900` | `#0B1B2D` |

#### 🌫️ Fog Gray（中性色 · 海雾灰）
带极淡青蓝调的冷灰，比纯灰多一份"湿润感"。

| Token | HEX | 用途 |
|-------|-----|------|
| `fog-0`   | `#FFFFFF` | 纯白 |
| `fog-50`  | `#F7FAFB` | 页面底色（浅） |
| `fog-100` | `#EEF2F4` | 分组底色 |
| `fog-200` | `#DDE4E8` | 边框 |
| `fog-300` | `#C3CDD3` | 弱边框 |
| `fog-400` | `#93A0A8` | 占位文字 |
| `fog-500` | `#6B7882` | 次级文本 |
| `fog-600` | `#49545D` | 副正文 |
| `fog-700` | `#2E373F` | 主文本（浅主题） |
| `fog-800` | `#1B222A` | 深色卡片 |
| `fog-900` | `#10161D` | 深色页面底 |
| `fog-950` | `#070B10` | 深色最深层 |

#### 🪸 Accent 辅色（海岸色盘）
饱和度适度提升，让界面更"活"，但仍控制在 ≤ 70%。

| Token | HEX | 命名 | 语义 |
|-------|-----|------|------|
| `coral-500`  | `#FF6B57` | Coral 珊瑚 | Danger / Highlight |
| `sunset-500` | `#F59E4B` | Sunset 晚霞 | Warning |
| `sand-500`   | `#E8C89A` | Sand 沙金 | Soft accent |
| `lime-500`   | `#A3D65C` | Lime 嫩松 | Success |
| `sky-500`    | `#4AB8E0` | Sky 晴海 | Info (Light) |
| `aurora-500` | `#7B6CFF` | Aurora 极光紫 | 特殊标签 / 数据可视化 |

> **饱和度原则**：主色 Teal 和 Coral 相对明亮，但其他色全部低饱和，确保在一屏并排也不刺眼。

### 2.2 语义色 Token（Semantic Tokens）

业务代码永远使用语义 Token，不直接使用原色。

#### ☀️ 浅色主题（Light · Coastal Morning · 海岸晨光）

| Token | 值 | 说明 |
|-------|----|------|
| `--color-bg`              | `fog-50`     | 页面底色 |
| `--color-bg-elevated`     | `fog-0`      | 卡片 / 浮层 |
| `--color-bg-sunken`       | `fog-100`    | 凹陷分组、代码块 |
| `--color-bg-overlay`      | `rgba(11,27,45,0.45)` | 遮罩 |
| `--color-border`          | `fog-200`    | 常规边框 |
| `--color-border-strong`   | `fog-300`    | 强调边框 |
| `--color-text`            | `fog-800`    | 正文 |
| `--color-text-secondary`  | `fog-600`    | 次级文本 |
| `--color-text-muted`      | `fog-500`    | 辅助说明 |
| `--color-text-disabled`   | `fog-400`    | 禁用 |
| `--color-text-on-primary` | `fog-0`      | 主色上文字 |
| `--color-primary`         | `teal-500`   | 主品牌 |
| `--color-primary-hover`   | `teal-600`   | |
| `--color-primary-active`  | `teal-700`   | |
| `--color-primary-soft`    | `teal-100`   | 主色软背景 |
| `--color-accent`          | `coral-500`  | 强调/引导 |
| `--color-success`         | `lime-500`   | |
| `--color-warning`         | `sunset-500` | |
| `--color-danger`          | `coral-500`  | |
| `--color-info`            | `sky-500`    | |

#### 🌙 深色主题（Dark · Deep Sea Night · 深海之夜）

| Token | 值 | 说明 |
|-------|----|------|
| `--color-bg`              | `#07101A`    | 略带深海蓝的近黑 |
| `--color-bg-elevated`     | `#0F1C28`    | 卡片 |
| `--color-bg-sunken`       | `#050B12`    | 凹陷 |
| `--color-bg-overlay`      | `rgba(2,8,15,0.65)` | |
| `--color-border`          | `#1E2C3A`    | |
| `--color-border-strong`   | `#2E4253`    | |
| `--color-text`            | `#E4EEF2`    | 正文（不用纯白） |
| `--color-text-secondary`  | `#A3B4BE`    | |
| `--color-text-muted`      | `#6D7E89`    | |
| `--color-text-disabled`   | `#47545E`    | |
| `--color-text-on-primary` | `#042A22`    | 深字配亮主色 |
| `--color-primary`         | `#3BDDBE`    | 深色下提亮的海松青 |
| `--color-primary-hover`   | `#5FE8CD`    | |
| `--color-primary-active`  | `#84F0D8`    | |
| `--color-primary-soft`    | `rgba(59,221,190,0.12)` | |
| `--color-accent`          | `#FF8370`    | |
| `--color-success`         | `#B5E066`    | |
| `--color-warning`         | `#FFB366`    | |
| `--color-danger`          | `#FF8370`    | |
| `--color-info`            | `#6DCCEF`    | |

> **深色原则**：绝不用纯黑。底色是"深海蓝黑"，让夜色里仍有海的气息；主色提亮 30% 以上，保证在深底上足够醒目。

### 2.3 特色渐变（Signature Gradients）

SeaForest 的视觉特色来自几组招牌渐变：

```css
--gradient-aurora:   linear-gradient(135deg, #0E9F86 0%, #4AB8E0 55%, #7B6CFF 100%);
--gradient-coastal:  linear-gradient(135deg, #0E9F86 0%, #2C5E96 100%);
--gradient-sunrise:  linear-gradient(135deg, #FF6B57 0%, #F59E4B 50%, #E8C89A 100%);
--gradient-seafoam:  linear-gradient(135deg, #ECFBF7 0%, #CFF4EA 50%, #D5E4F4 100%);
--gradient-deepsea:  radial-gradient(ellipse at top, #2C5E96 0%, #0B1B2D 70%);
```

---

## 3. 字体系统（Typography）

SeaForest 采用**跨端统一的开源字体方案**：西文沿用硅谷开源三剑客 Inter / Space Grotesk / JetBrains Mono；中文统一使用华为开源的 **HarmonyOS Sans SC**——它几何感强、字面干净、与西文的 Inter/Space Grotesk 气质一致，且在 Windows / macOS / Linux / Android / iOS 上都能获得完全相同的视觉体验。

```css
--font-sans:    "Inter", "HarmonyOS Sans SC", system-ui, -apple-system, "PingFang SC", sans-serif;
--font-display: "Space Grotesk", "HarmonyOS Sans SC", "Inter", sans-serif;
--font-mono:    "JetBrains Mono", "Fira Code", "SF Mono", Menlo, Consolas, monospace;
```

- **Sans**（Inter + HarmonyOS Sans SC）：正文与 UI，字形干净、宽松、现代
- **Display**（Space Grotesk + HarmonyOS Sans SC）：Hero / 标题，带几何感，让品牌更年轻
- **Mono**（JetBrains Mono + 系统等宽）：代码与 Token，向开发者文化致敬（HarmonyOS Sans 没有官方等宽版本，Mono 场景不混入中文栈）

### 字体加载（CDN 方式）

为了零配置、开箱即用，preview.html 通过 **jsDelivr + `@lobehub/webfont-harmony-sans-sc`** 一行 `<link>` 加载 HarmonyOS Sans SC，无需管理本地字体文件：

```html
<link rel="preconnect" href="https://cdn.jsdelivr.net" crossorigin />
<link href="https://cdn.jsdelivr.net/npm/@lobehub/webfont-harmony-sans-sc@1.0.0/css/index.min.css" rel="stylesheet" />
```

- 包体由 LobeHub 团队维护并发布到 npm，jsDelivr 全球 CDN 分发，国内访问稳定
- family name 为 `"HarmonyOS Sans SC"`（**带 SC 后缀**），含完整的 GB2312/GB18030 中文字形
- 打包 4 档字重：`300 Light` / `400 Regular` / `500 Medium` / `700 Bold`，每档 woff2 约 4 MB
- CSS 自带 `font-display: swap` 与 `local(...)` 声明：本机已装 HarmonyOS Sans SC 时会优先用本地副本，省流量

> **兵底策略**：如果 CDN 不可达（比如内网环境、墙），`--font-sans` 中定义的 fallback 链会自动启用 → Inter → system-ui → PingFang SC（macOS）/ 微软雅黑（Windows），站点可用性不受影响。
### 生产环境建议

CDN 方案适合**原型、Demo、个人项目**；如果是对可用性 / 性能敏感的生产环境，建议改为**自托管 + 子集化**：

1. 从华为开发者官网下载：<https://developer.huawei.com/consumer/cn/design/resource/>
2. 用 [fontmin](https://github.com/ecomfe/fontmin) 或 [cn-font-split](https://github.com/KonghaYao/cn-font-split) 按 unicode-range 子集化，正文字重单文件可从 ~6MB 压到 ~600KB
3. 放到自家 CDN / OSS，用 `@font-face` 引入，`font-display: swap` 避免阻塞渲染

### Type Scale

| Token | Size | Line | Letter | 用途 |
|-------|------|------|--------|------|
| `display-1` | 64px | 1.05 | -0.03em | Hero 超大标题 |
| `display-2` | 48px | 1.1  | -0.025em | 二级 Hero |
| `h1`        | 34px | 1.2  | -0.02em | 页面标题 |
| `h2`        | 26px | 1.3  | -0.015em | 分区 |
| `h3`        | 20px | 1.4  | -0.01em | 卡片 |
| `h4`        | 17px | 1.5  | 0 | 子标题 |
| `body-lg`   | 16px | 1.65 | 0 | 长文 |
| `body`      | 14px | 1.6  | 0 | 默认 |
| `body-sm`   | 13px | 1.55 | 0 | 次要 |
| `caption`   | 12px | 1.5  | 0.01em | 标签 |
| `code`      | 13px | 1.6  | 0 | 代码 |

> 与上一版相比：Hero 字号放大、字间距收紧，视觉冲击更强；辅助文字略微"轻"一点，突出内容层级。

---

## 4. 间距与布局（Spacing & Layout）

### 4.1 Spacing（4px 基准）

| Token | 值 |
|-------|----|
| `space-1`  | 4px |
| `space-2`  | 8px |
| `space-3`  | 12px |
| `space-4`  | 16px |
| `space-5`  | 20px |
| `space-6`  | 24px |
| `space-8`  | 32px |
| `space-10` | 40px |
| `space-12` | 48px |
| `space-16` | 64px |
| `space-20` | 80px |
| `space-24` | 96px |
| `space-32` | 128px |

### 4.2 Breakpoints

| sm | md | lg | xl | 2xl |
|----|----|----|----|-----|
| 640 | 768 | 1024 | 1280 | 1536 |

---

## 5. 圆角（Radius）

SeaForest 偏爱"圆润但不卡通"的圆角，主控件比上一版稍大一点，更现代：

| Token | 值 | 用途 |
|-------|----|------|
| `radius-xs`   | 4px    | 标签 |
| `radius-sm`   | 8px    | 输入 |
| `radius-md`   | 12px   | **按钮、控件（默认）** |
| `radius-lg`   | 16px   | 卡片 |
| `radius-xl`   | 24px   | 弹窗、大容器 |
| `radius-2xl`  | 32px   | Hero |
| `radius-full` | 9999px | 胶囊 / 头像 |

---

## 6. 阴影与高度（Elevation）

### 浅色（带青色色调）

```css
--shadow-xs: 0 1px 2px rgba(11, 27, 45, 0.05);
--shadow-sm: 0 2px 8px -2px rgba(11, 27, 45, 0.08), 0 1px 2px rgba(11, 27, 45, 0.04);
--shadow-md: 0 8px 20px -6px rgba(11, 27, 45, 0.12), 0 2px 4px rgba(11, 27, 45, 0.05);
--shadow-lg: 0 20px 40px -12px rgba(11, 27, 45, 0.16), 0 6px 12px rgba(11, 27, 45, 0.06);
--shadow-xl: 0 32px 64px -16px rgba(11, 27, 45, 0.22), 0 10px 20px rgba(11, 27, 45, 0.08);
--shadow-glow:        0 0 0 4px rgba(14, 159, 134, 0.20);
--shadow-glow-coral:  0 0 0 4px rgba(255, 107, 87, 0.22);
--shadow-halo:        0 0 48px rgba(14, 159, 134, 0.22);  /* 光晕效果 */
```

### 深色（阴影 + 光晕并重）

```css
--shadow-xs: 0 1px 2px rgba(0,0,0,0.5);
--shadow-sm: 0 2px 8px rgba(0,0,0,0.5);
--shadow-md: 0 8px 24px rgba(0,0,0,0.55);
--shadow-lg: 0 20px 48px rgba(0,0,0,0.6);
--shadow-xl: 0 32px 80px rgba(0,0,0,0.7);
--shadow-glow:        0 0 0 4px rgba(59, 221, 190, 0.28);
--shadow-glow-coral:  0 0 0 4px rgba(255, 131, 112, 0.30);
--shadow-halo:        0 0 56px rgba(59, 221, 190, 0.25);
```

深色模式下，`--shadow-halo` 被大量使用以制造"深海夜光"质感。

---

## 7. 动效（Motion）

### Duration

| Token | 值 |
|-------|----|
| `duration-instant` | 80ms  |
| `duration-fast`    | 160ms |
| `duration-base`    | 220ms |
| `duration-slow`    | 360ms |
| `duration-slower`  | 520ms |

### Easing

```css
--ease-standard:   cubic-bezier(0.2, 0.6, 0.2, 1);    /* 默认 */
--ease-emphasized: cubic-bezier(0.3, 0.8, 0.2, 1);    /* 进入 */
--ease-exit:       cubic-bezier(0.4, 0, 1, 1);        /* 退出 */
--ease-spring:     cubic-bezier(0.34, 1.56, 0.64, 1); /* 轻弹性 */
--ease-wave:       cubic-bezier(0.45, 0.05, 0.55, 0.95); /* 潮汐 */
```

### 招牌动效

1. **潮汐呼吸**（Wave Breathing）：长留组件（如 Hero、空态）可使用 `wave` 曲线的 3–4s 循环，让背景像潮水一样缓缓起伏。
2. **光波扫过**（Light Sweep）：主按钮 hover 时从左到右扫过一层微光。
3. **浮升反馈**：卡片 hover 轻微上浮 2–4px，同时阴影从 sm → md。

---

## 8. 组件规范（Components）

### 8.1 Button
- 变体：`primary` / `secondary` / `ghost` / `danger` / `accent`（Coral 强调行动）
- 尺寸：`sm 32` / `md 40` / `lg 48`
- **特色**：主按钮使用 Aurora / Coastal 渐变背景 + 微微光晕，在深色下更明显
- 支持 hover 时的光波扫过效果

### 8.2 Input
- 高度 40 / 圆角 `radius-md`
- 聚焦：边框变 primary + 4px glow（发光环）
- 错误态：Coral 边框 + Coral helper

### 8.3 Card
- 背景：`--color-bg-elevated`
- 可选**玻璃拟态版本**：`backdrop-filter: blur(20px)` + 半透明背景
- hover：上浮 2px + 阴影 md
- 允许使用 aurora 渐变作为装饰顶条或角光

### 8.4 Dialog / Modal
- 圆角 `radius-xl`，阴影 xl
- **遮罩带 backdrop-blur(12px)**，制造海雾感

### 8.5 Code Block
- 背景 `--color-bg-sunken`
- 语法高亮：关键字 teal / 字符串 sunset / 注释 muted / 数字 aurora

### 8.6 Badge / Tag
- 胶囊形，软背景 + 前缀点
- 颜色：primary / success / warning / danger / info / accent

---

## 9. 图标与插画

- **尺寸**：16 / 20 / 24
- **线宽**：1.5px，端点圆头
- **风格**：几何 + 有机弧度（Lucide / Phosphor Regular）
- **插画**：允许 noise 纹理、aurora 渐变；在 Hero 和空态中使用海浪/波纹/松针等元素

---

## 10. 数据可视化

- **色序**：`teal-500 → aurora-500 → sky-500 → sunset-500 → coral-500 → lime-500 → sand-500`
- 网格用 dashed `--color-border`
- 面积图填充用 teal 到透明的渐变，营造"海面倒影"
- 悬停 tooltip 使用玻璃拟态卡片

---

## 11. 可访问性

- 文本对比度 ≥ 4.5:1（WCAG AA）
- 聚焦环统一 4px glow，不用边框颜色变化单独表达
- 支持 `prefers-reduced-motion` / `prefers-color-scheme`
- 禁用色不仅靠透明度，还需要状态图标辅助

---

## 12. 使用原则

1. **Token First**：永远使用语义 Token。
2. **渐变克制**：Aurora / Coastal 渐变是品牌印记，单屏内 ≤ 2 处。
3. **Coral 是调味料**：珊瑚橙是 SeaForest 的"活"感来源，但一屏中只在**最重要的一个 CTA**使用。
4. **玻璃拟态要"有东西可模糊"**：只在背景有层次（如渐变、图片）时使用 backdrop-blur。
5. **深浅等价不等同**：深色不是浅色的反色，它有自己的情绪（深海之夜）。

---

## 13. 版本

- **v0.1.0 · Tide** — 海松青主色、珊瑚橙强调、极光渐变、玻璃拟态、现代的字号节奏。

> 🌊🌲 SeaForest 相信：**最美的森林，在海边。**
