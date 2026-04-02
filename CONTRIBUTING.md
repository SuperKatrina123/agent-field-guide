# Contributing to Agent Field Guide

欢迎共建！Agent Field Guide 是一本关于 Agent 工程的开放参考手册，我们欢迎以下三种贡献：

| 类型 | 描述 | 对应 Issue 模板 |
|------|------|----------------|
| 📚 **知识点补充** | 补充某个主题的知识点，可附流程图 | `knowledge` |
| 🔧 **踩坑经验** | 开发过程中遇到的真实问题与解法 | `case` |
| 🎯 **面试题** | Agent 相关面试题及解析 | `interview` |

---

## 快速开始

1. **Fork** 本仓库
2. 新建分支：`git checkout -b feat/your-topic`
3. 参考 [STYLE-GUIDE.md](STYLE-GUIDE.md) 写内容
4. 提交 PR，填写 PR 模板

---

## 贡献到哪里

| 贡献类型 | 目标文件 |
|---------|---------|
| 知识点补充 | 对应的 `01–17` 章节文件，或新建子文档 |
| 踩坑经验 | `15-案例研究与拆解.md` |
| 面试题 | `18-面试题库.md`（如不存在请新建） |

---

## 流程图贡献约定

我们鼓励为知识点配流程图，推荐以下工具：

| 工具 | 格式 | 说明 |
|------|------|------|
| **Excalidraw** | `.excalidraw` | 首选，风格统一，可在 Obsidian 中直接渲染 |
| **Mermaid** | 代码块 ` ```mermaid ` | 在 GitHub 上原生渲染，无需额外文件 |
| **draw.io** | 导出为 `.svg` 后放入对应章节 `assets/` 目录 | 备选 |

**Excalidraw 风格约定**（保持与现有图表一致）：
- `roughness: 0`，`fillStyle: "solid"`
- 字体：Helvetica（`fontFamily: 2`）
- 矩形圆角：`{"type": 3}`，箭头圆角：`{"type": 2}`

---

## 写作规范

所有贡献必须遵循 [STYLE-GUIDE.md](STYLE-GUIDE.md)，核心原则：

- 使用约定好的 6 类 Callout（定义 / 原则 / 方法 / 误区 / 案例 / 练习）
- H1 只用于标题，H2 一级模块，H3 子主题，不使用 H4
- 内链克制，列表项简洁
- 提交前完成 STYLE-GUIDE 中的检查清单

---

## 提交规范

```
feat: 在 07-状态管理 补充向量记忆检索流程图
fix: 修正 03-上下文工程 中的错误描述
case: 新增 RAG 召回率低的踩坑经验
interview: 新增多 Agent 通信面试题
```

---

## 行为准则

- 保持内容客观，有依据
- 踩坑经验请描述真实场景，避免泛泛而谈
- 面试题请附上解析，不只是问题
- 尊重已有内容结构，大改动请先开 Issue 讨论
