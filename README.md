# 🚀 LoadingMarker 动画生成器

**项目简介**：
一款基于浏览器端（HTML5 Canvas + WASM）的高性能 Loading 动画生成工具。支持实时预览、多模版切换、颜色深度定制以及 GIF/APNG 双格式导出，专为前端开发者和 UI 设计师打造。

---

### 📦 v2.0.0 (Final Release) - 2025.11.26
**里程碑：正式上线 / GitHub Pages 部署**
- **[部署]** 完成静态资源打包，成功部署至 GitHub Pages，支持公网访问。
- **[优化]** 统一界面布局，左侧参数面板与右侧预览区域高度自适应对齐。
- **[优化]** 输出格式与压缩等级控件分行显示，增加数值百分比外显，交互更直观。
- **[新增]** 底部增加版权署名 (Designed by NevenHhhhh)。
- **[修复]** 修复了 input range 在不同浏览器下的样式兼容性问题（`appearance` 属性警告）。

### ✨ v1.5.0 (Advanced Color) - 高级色彩与背景
**核心升级：全自定义背景支持**
- **[新增]** 背景控制面板：支持“透明背景”开关。
- **[新增]** 背景色支持 RGBA：允许用户自定义背景颜色 + 透明度（Alpha通道），解决 GIF 边缘锯齿问题。
- **[新增]** 智能 HEX 输入：支持手动输入颜色代码（如 `#FF0000` 或 `FF0000`），并与色盘双向同步。
- **[交互]** 增加了针对 GIF 格式不支持半透明背景的智能提示（Tooltip）。

### 🎨 v1.2.0 (UI/UX Polish) - 视觉与交互重构
**核心升级：CSS Grid 布局与控件美化**
- **[重构]** 使用 CSS Grid 重写整体布局，解决 flex 布局下的挤压问题。
- **[美化]** 自定义重绘了原生 `<input type="color">` 和 `<input type="range">`，使其在各浏览器下风格统一且美观。
- **[新增]** 强制 1:1 正方形尺寸限制，移除繁琐的宽高单独设置，简化操作。

### 🛠 v1.0.0 (Core Features) - 功能增强
**核心升级：模版库扩充与压缩算法**
- **[新增]** 内置 7 种主流 Loading 模版：
  - `iOS Spinner` (经典菊花)
  - `Smooth Ring` (平滑圆环)
  - `Chasing Dots` (追逐圆点)
  - `Equalizer` (音律跳动)
  - `Pulse` (脉冲扩散)
  - `Fading Circle` (淡入圆圈)
  - `Bouncing Dots` (三点跳动)
- **[新增]** 帧率 (FPS) 控制器 (10-60fps)，提供更高效的体积压缩方案。
- **[优化]** 重写 GIF/APNG 压缩逻辑，支持通过减少色彩数 (Quantization) 大幅降低文件体积。

### 🌱 v0.1.0 (Prototype) - 原型验证
**核心升级：MVP (最小可行性产品)**
- **[基础]** 搭建 HTML5 Canvas 绘图引擎。
- **[核心]** 引入 `gif.js` 和 `upng.js` 实现前端生成动图。
- **[功能]** 实现基础的旋转动画导出。

---

### 💻 技术栈 (Tech Stack)
*   **Core**: HTML5, CSS3, Vanilla JavaScript (ES6+)
*   **Rendering**: Canvas 2D API
*   **Encoding**:
    *   `gif.js` (GIF encoding via Web Workers)
    *   `upng-js` (High-quality APNG encoding with compression)
*   **Deployment**: GitHub Pages

---

### 👨‍💻 Author
Designed & Developed by **NevenHhhhh**
