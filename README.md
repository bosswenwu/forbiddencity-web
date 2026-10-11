# 紫禁城 · 数字漫游

这是接管重制后的浏览器版主交付：以故宫中轴为骨架的实时 3D 漫游，不依赖下载的模型或贴图。

## 启动

在 PowerShell 中运行：

\`\`\`powershell
Set-Location "D:\AI项目\03_3D与建模\紫禁城\ForbiddenCity-Web"
npm start
\`\`\`

然后打开 <http://localhost:8765/index.html>。页面需要联网加载 Three.js。

公网地址：<https://bosswenwu.github.io/forbiddencity-web/>

## 体验内容

- 11 个中轴地标：午门、金水桥、太和门、太和殿、中和殿、保和殿、乾清门、乾清宫、交泰殿、坤宁宫、御花园。
- 三种浏览方式：自由漫游、逐处导览、全景俯瞰。
- 桌面操作：WASD 移动，Shift 加速，鼠标环视，M 隐藏/显示界面。
- 手机操作：左侧虚拟摇杆移动，拖动画面环视，右侧按钮登高或跳到下一处。
- 程序化建筑细节：曲面庑殿意象屋顶、重檐、柱廊、汉白玉台基与栏杆、城墙、护城河、金水桥、配殿、树木和宫灯。

本项目是风格化互动作品，不是测绘级数字孪生；地标文字用于导览，空间与造型做了适合实时浏览的简化。

## 自检

保持本地服务器运行后，在另一个 PowerShell 窗口执行：

\`\`\`powershell
Set-Location "D:\AI项目\03_3D与建模\紫禁城\ForbiddenCity-Web"
npm run verify
\`\`\`

脚本会真实执行键盘移动、地标切换、全景切换和手机虚拟摇杆，并检查 console/page error、移动端溢出和调试状态；验收截图写入 \`screenshots\`。

需求与验收口径见 [SPEC.md](./SPEC.md)。
