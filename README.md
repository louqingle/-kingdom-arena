# 王者战域 · Kingdom Arena

面向手机浏览器的 3D 斜俯视 5V5 推塔游戏原型。

## 当前玩法
- 单人操控蓝方战士，红蓝双方共 10 名英雄
- 三路战场、自动推进的兵线、双方防御塔和基地水晶
- iPhone 触屏虚拟摇杆、普攻、范围技能、位移和回城
- 自动跟随镜头、横屏提示、击杀/金币/生命与法力 HUD
- GitHub Actions 自动发布 GitHub Pages

## 操作
横屏打开网页；左侧摇杆移动，右侧普攻持续攻击，技能 1 造成范围伤害，技能 2 位移，回城恢复状态。先清理敌方英雄和兵线，再摧毁敌方三座防御塔，最后攻击水晶。

## 发布
仓库根目录的 `index.html` 是入口。推送到 `main` 会触发 `.github/workflows/pages.yml` 发布。首次发布前需在仓库 Settings → Pages 中将 Build and deployment 的 Source 设为 GitHub Actions。

## 技术说明
Three.js 通过 CDN 加载，首次运行需要网络。当前为持续开发中的可玩原型，不代表完整商业级 MOBA 成品；后续将继续完善角色模型、技能特效、寻路、兵线与防御塔策略、音效和性能。