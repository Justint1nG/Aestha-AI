# Aestha — Fitting Room

可点击的 iOS 风格浏览器原型。双击 `index.html` 即可使用；也可以通过任意静态文件服务器运行。无需安装依赖。

## 已实现

- 五类商品切换、可横滑商品列表和前后切换按钮。
- 四套外套示例穿搭切换。
- 收藏穿搭及重新打开收藏。
- 尺码选择、加入演示购物袋、金额合计和移除商品。
- 手机布局和桌面手机框展示。

## 演示边界

这不是原生 SwiftUI 工程，不能直接提交 App Store。图片、价格和商品为示例。只有外套切换会更换中央示例图；其他类别支持选款和加入购物袋，不会生成新的试穿图。未接入 AI、账户、支付或真实库存。收藏与购物袋仅保留在当前页面会话中，刷新会重置。Google Fonts 不可用时会自动使用系统字体。

## 文件

- `index.html`：界面结构
- `style.css`：响应式样式
- `app.js`：商品、收藏、购物袋交互
- `looks.png`：示例穿搭素材

## 图片制作

通过内置 imagegen 生成；未使用 CLI。生成提示词如下：

Create one photorealistic fashion contact sheet, landscape 3:2 ratio, exactly FOUR equal-width vertical panels side by side, no gaps or borders, no text, no UI. Each panel shows the same handsome adult East Asian male model age 25, same face, full body from hair to soles, centered, standing straight relaxed with arms by sides, charcoal concrete fashion studio with soft warm overhead spotlight and dark gray floor. Each panel has ample blank space above head and below shoes, model occupies 80 percent of height. Panel 1: black leather zip utility jacket over white tee, wide black cargo pants and black white sneakers. Panel 2: slate blue denim trucker jacket over white tee, same black cargo pants and sneakers. Panel 3: olive green technical parka over white tee, same black cargo pants and sneakers. Panel 4: black hooded bomber jacket over white tee, same pants and sneakers. Premium Korean streetwear editorial, subdued cinematic light yet clothes are visible and textured, realistic natural human anatomy. This is an image asset atlas for an interactive fitting room, keep exactly four equally sized columns with the model fully contained within each column. No typography.

## 验证

已检查 JavaScript 语法。已在浏览器验证外套切换、收藏状态、尺码面板、加入购物袋、金额和移除商品；390 × 844 布局无横向溢出，底部导航与 home indicator 均在视口内。
