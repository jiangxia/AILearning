# 内容框架规范

## 📝 文档元数据标准

### 必需字段（frontmatter）
每篇文章必须包含以下元数据：

```yaml
---
# 4P层级定位
layer: Products/Practice/Protocol/Pattern

# Diátaxis文档类型
type: Tutorial/How-to/Explanation/Reference

# PSO框架
purpose: "明确描述文档要解决的具体问题"
scope:
  includes: 
    - "必须包含的内容要点1"
    - "必须包含的内容要点2"
  excludes:
    - "明确排除的内容1"
    - "明确排除的内容2"
outcome:
  - "读者能获得的具体能力1"
  - "读者能获得的具体能力2"

# 基础信息
title: "文章标题"
date: YYYY-MM-DD
author: "黄明易"
category: "AI学习"
tags: ["AI工具", "学习指南", "实践方法"]
status: draft/published
version: "1.0"

# 可选字段
difficulty: beginner/intermediate/advanced
estimated_time: "阅读时间估计"
prerequisites: ["前置要求1", "前置要求2"]
related_articles: ["相关文章链接"]
---
```

## 📁 目录结构规范

### 4P分层目录
```
content/
├── 01-products/                 # AI工具实战
│   ├── index.md                # 目录索引
│   ├── chatgpt/                # ChatGPT相关
│   ├── claude/                 # Claude相关
│   ├── specialized-tools/      # 专业工具
│   └── comparisons/           # 工具对比
├── 02-practice/                # AI协作方法
│   ├── index.md
│   ├── prompt-engineering/     # Prompt工程
│   ├── workflow-design/        # 工作流设计
│   ├── collaboration-methods/  # 协作方法
│   └── quality-control/       # 质量控制
├── 03-protocol/                # AI交互设计
│   ├── index.md
│   ├── interaction-patterns/   # 交互模式
│   ├── communication-protocols/ # 通信协议
│   ├── structure-design/       # 结构设计
│   └── interface-standards/   # 接口标准
└── 04-pattern/                 # AI哲学思考
    ├── index.md
    ├── cognitive-theory/       # 认知理论
    ├── ethics-philosophy/      # 伦理哲学
    ├── future-thinking/        # 未来思考
    └── legal-implications/     # 法律启示
```

### 文件命名规范
- **格式**：`主题-子主题-类型.md`
- **示例**：
  - `chatgpt-legal-research-howto.md`
  - `prompt-engineering-best-practices-reference.md`
  - `ai-consciousness-philosophical-explanation.md`

## 📊 4P层级与Diátaxis类型配合

### Products层（优先组合）
- **主要类型**：How-to（60%）+ Tutorial（30%）
- **次要类型**：Reference（10%）
- **特点**：实操性强，立即可用

### Practice层（优先组合）
- **主要类型**：Reference（50%）+ How-to（40%）
- **次要类型**：Explanation（10%）
- **特点**：标准化，可复制

### Protocol层（优先组合）
- **主要类型**：Explanation（60%）+ Reference（30%）
- **次要类型**：How-to（10%）
- **特点**：原理性强，系统理解

### Pattern层（优先组合）
- **主要类型**：Explanation（80%）+ Reference（20%）
- **次要类型**：无
- **特点**：思辨性强，启发思考

## ✍️ 写作质量标准

### Tutorial类型要求
- **开头**：明确学习目标和前置条件
- **结构**：步骤清晰，循序渐进
- **实践**：提供具体练习和验证方法
- **结尾**：总结要点，指引下一步学习

### How-to类型要求
- **开头**：直接说明要解决的问题
- **步骤**：编号清晰，可操作性强
- **案例**：提供具体的应用场景示例
- **故障排除**：预料常见问题和解决方案

### Explanation类型要求
- **背景**：解释为什么需要理解这个概念
- **原理**：深入浅出地说明核心机制
- **关联**：连接到读者已知的概念
- **启示**：提供思考角度和应用方向

### Reference类型要求
- **组织**：信息结构化，易于查找
- **完整性**：覆盖主题的各个方面
- **准确性**：信息准确，来源可靠
- **更新性**：标明版本和更新时间

## 🎯 内容质量检查清单

### 基础要求（必须满足）
- [ ] 元数据完整且符合规范
- [ ] PSO框架明确定义
- [ ] 4P定位准确
- [ ] 文档类型符合层级特点
- [ ] 标题吸引人且准确
- [ ] 结构清晰，逻辑连贯

### 实用性要求
- [ ] 有具体的应用场景
- [ ] 提供可操作的步骤或方法
- [ ] 包含实际案例或示例
- [ ] 读者看完能立即行动

### 专业性要求
- [ ] 术语使用准确
- [ ] 避免AI味的表达
- [ ] 体现AI学习的深度
- [ ] 信息来源可靠

### 用户体验要求
- [ ] 长度适中（1000-2000字）
- [ ] 排版清晰，易于阅读
- [ ] 关键点突出标记
- [ ] 提供相关链接和延伸阅读

## 📚 写作模板应用

### 选择模板的决策树
1. **确定4P层级** → 选择主要文档类型
2. **明确具体目标** → 选择对应模板
3. **考虑读者水平** → 调整内容深度
4. **评估时间资源** → 确定内容范围

### 模板使用原则
- 模板是指导，不是限制
- 根据具体内容灵活调整
- 保持PSO框架的一致性
- 确保实用性和可操作性

## 🔄 内容演进机制

### PDCA持续改进
- **Plan**：根据读者反馈制定改进计划
- **Do**：实施内容更新和优化
- **Check**：评估改进效果
- **Act**：固化有效的改进措施

### 版本管理
- 重大更新：version +1.0
- 内容补充：version +0.1
- 修正错误：version +0.01

---
*基于deepractice内容规范体系设计*
*版本：v1.0 | 更新时间：2025-01-21*