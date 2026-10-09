# 廿四 · 节气之轮

> 一座可以转动的二十四节气罗盘 —— 廿四次呼吸，转完中国人的一年。

**在线体验**：[GitHub Pages](https://bidepanwin.github.io/24-solar-terms/)

## 玩法

- **拖动罗盘**旋转（带惯性与磁吸），转到哪个节气，整站主题色与全屏天象粒子随之切换
- **天象系统**：雨水落雨、惊蛰雷暴闪电、小雪大雪飘雪、清明飘花瓣、大暑萤火漫天、霜降霜花与红叶……9 种粒子行为交叉过渡
- **今日节气**自动识别：罗盘定位、卡片「今日」标记、页脚一年进度
- 支持点击节气名跳转、`←` `→` 键盘切换；粒子会被鼠标推开
- 彩蛋：小满时节的金色光尘会慢慢「将满未满」地涨大

## 技术

单文件 `index.html`，纯原生 HTML / CSS / JavaScript + Canvas，零依赖、零构建。

- Pointer Events 拖拽 + `setPointerCapture`，角度环绕与吸附物理
- Canvas 粒子引擎：配置驱动的分层粒子 + 衰亡重生式场景过渡
- `IntersectionObserver` 滚动显现、`prefers-reduced-motion` 降级、DPR 适配、移动端触控

## License

MIT
