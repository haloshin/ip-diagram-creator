# 安全、授权与资产放置规则

## 授权原则

默认只处理用户明确授权提供的材料：

- 本人照片或本人账号截图。
- 用户拥有管理权的品牌主页。
- 用户自己写的简介、文章、课程大纲、脚本。
- 用户有权使用的参考图或版式示例。

如果材料涉及他人头像、私信、客户资料、后台数据或联系方式，先提醒用户打码、裁切或改用摘要。

## 隐私边界

不要要求用户上传不必要的敏感材料。以下内容不应进入普通图解流程：

- 身份证件、住址、电话号码、银行卡等敏感信息。
- 私密聊天记录。
- 后台账号、财务数据、订单明细。
- 未授权的员工、客户、学生或第三方肖像。
- 未公开的商业资料。

## 参考图版权边界

公共 Skill 包里只放：

- 自己创作且允许公开分发的参考图。
- 明确授权公开分发的素材。
- 文字描述、版式说明和抽象结构。

不要把平台截图、课程截图、商业海报、设计网站图片或他人作品直接放进仓库。可以用文字描述它们的结构，但不要复刻具体构图、角色、品牌元素或商业视觉。

## 两类资产不要混放

Skill 包里的图分两类：

1. **通用参考图**：帮助 Skill 判断视觉模式、信息量和知识卡形态。
2. **用户角色资产**：某个用户建档后生成的长期固定资产。

通用参考图可以随 Skill 分发；用户角色资产属于具体用户或项目，不应作为所有用户默认资产。

## 通用参考图建议目录

```text
assets/examples/
  illustration-density/
    low-density.png
    mid-density.png
    high-density.png
  knowledge-cards/
    workflow-card.png
    comparison-card.png
    checklist-card.png
    framework-card.png
    diagnosis-card.png
```

规则：

- 低 / 中 / 高信息量参考图只服务手绘插图模式。
- 知识卡参考图不要按信息量分类，按信息结构分类。
- 知识卡参考图只是样本，不是固定模板。
- 出图时不能复刻参考图构图，要根据当前内容创造合适形态。

## 角色资产版式示例

建议放在：

```text
assets/templates/character-assets/
  character-main-anchor-example.png
  character-spec-board-example.png
  character-action-expression-small-scene-example.png
```

这些只是版式示例，用来说明三张角色资产应该长什么样。

## 用户角色资产

某个用户确认后的三张角色资产，建议保存到用户或项目自己的输出目录：

```text
outputs/{user_or_project}/character-assets/
  01-character-main-anchor.png
  02-character-spec-board.png
  03-action-expression-small-scene.png
```

公共发行包不应包含任何真实用户角色资产。

## 后续调用规则

- 普通内容图：角色主锚图。
- 手绘插图模式、大场景、小比例人物：角色主锚图 + 动作 / 表情 / 小比例场景扩展图 + 对应手绘插图参考图。
- 知识卡模式：角色主锚图 + 对应知识卡结构参考图；复杂动作时补动作扩展图。
- 返修纠偏：角色规范说明图。
