# 前端技术选型指南

## 快速选择

### 🎯 根据项目类型选择

**Web应用**
- 营销网站/内容网站 → `Next.js` / `Nuxt.js`
- 管理后台/企业应用 → `React` / `Vue` SPA
- 复杂交互应用 → `React` 生态

**移动应用**
- iOS + Android 跨平台 → `cross-platform-flutter`
- iOS 专属应用 → `ios-swift`
- Web技能复用 → `React Native`

**桌面应用**  
- 跨平台桌面 → `frontend-electron`
- Mac专属应用 → `ios-swift`
- 性能敏感桌面应用 → `Tauri` / 原生

### 🚀 根据团队技能选择

**前端团队 (React/Vue背景)**
- 移动端需求 → `cross-platform-flutter` 或 `React Native`
- 桌面端需求 → `frontend-electron`
- Web端需求 → 继续使用现有技术栈

**全栈团队**
- 优先考虑统一技术栈 → `React` 全家桶
- 快速原型验证 → `cross-platform-flutter`

**移动开发团队**
- iOS专长 → `ios-swift`
- Android专长 → 考虑 `Kotlin` 或 `cross-platform-flutter`

### ⚡ 根据性能要求选择

**极致性能要求**
- 移动端 → `ios-swift` (iOS) + `Kotlin` (Android)
- 桌面端 → 各平台原生

**平衡需求** 
- 移动端 → `cross-platform-flutter`
- 桌面端 → `frontend-electron` 或 `Tauri`

**快速开发**
- 所有平台 → `cross-platform-flutter`
- 仅桌面 → `frontend-electron`

## Agent使用流程

### 1. 技术选型阶段
```bash
# 使用技术选型专家分析需求
@frontend-tech-selector

# 输入项目信息：
- 目标平台 (Web/iOS/Android/Desktop)
- 团队技能背景
- 性能要求
- 开发周期
- 维护期望
```

### 2. 开发执行阶段
根据选型结果，使用对应的专业Agent：

```bash
# Flutter跨平台开发
@cross-platform-flutter

# Electron桌面应用开发  
@frontend-electron

# Swift原生iOS/macOS开发
@ios-swift
```

### 3. 技术演进阶段
- 定期评估技术选型效果
- 必要时进行技术栈迁移
- 使用技术选型专家重新评估

## 决策矩阵

| 场景 | 首选方案 | Agent | 备选方案 |
|------|---------|-------|----------|
| 创业公司MVP | Flutter | `cross-platform-flutter` | React Native |
| 企业内部工具 | Electron | `frontend-electron` | Web应用 |
| iOS App Store应用 | Swift原生 | `ios-swift` | Flutter |
| 游戏/高性能应用 | Flutter/原生 | `cross-platform-flutter`/`ios-swift` | Unity |
| 内容管理网站 | Next.js | 待创建 | Nuxt.js |

## 常见问题

**Q: 什么时候选择原生开发？**
A: 需要平台特有功能、极致性能要求、或应用商店策略要求时。

**Q: 跨平台方案的主要风险？**  
A: 平台特异性功能支持、性能天花板、调试复杂度。

**Q: 如何处理技术栈迁移？**
A: 渐进式迁移、功能对等验证、团队培训并行进行。

**Q: 团队技能不匹配怎么办？**
A: 优先培训现有团队，或考虑混合开发策略。