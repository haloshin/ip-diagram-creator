# Prompt 模板

以下模板可以按图像生成模型调整。重点不是固定措辞，而是保留角色锚点、内容结构、视觉模式和安全边界。

## 01 角色主锚图

```text
Create one primary character anchor sheet for a creator's stable minimalist hand-drawn diagram persona.

Purpose:
This is the PRIMARY identity reference for all future content diagrams. It is not a commercial poster, not a dense infographic, and not a pretty-but-unusable avatar showcase.

Creator identity:
- Display name: {称呼}
- Field / profession: {领域/职业}
- Short bio: {简介}
- Desired vibe: {气质}

Identity anchors to preserve:
- Face / overall impression: {脸部与整体气质}
- Hair: {发型}
- Glasses / accessories: {眼镜或配饰}
- Outfit: {稳定服装}
- Body language: {体态}
- Expression: {常态表情}
- Color accents: {个人点缀色}

Visual style:
Pure white background. Beautiful minimalist black hand-drawn line art. Slightly wobbly but clean pen lines. Refined creator IP character feeling, aesthetically pleasing and memorable. Adult creator proportions simplified for diagram use. Polished enough to be lovable, but still diagram-friendly. Not realistic portrait, not chibi, not cute mascot, not ugly rough doodle, not stiff business portrait, not glossy illustration, not commercial poster.

Sheet layout:
1. One large main 3/4 view persona. Make the person large and clear.
2. 2-3 smaller views: front, 3/4, side.
3. 3-5 small identity anchor callouts: hair, glasses/accessory, outfit, expression, posture.
4. Minimal color accent swatches if useful.

Chinese labels:
Use short, clean Chinese handwritten labels only. Keep labels readable and sparse.

Avoid:
Do not make the person look like a child. Do not make it ugly, stiff, overly corporate, too cute, too polished, too commercial, too realistic, or too complex. Do not add complex background. Do not add unrelated people.
```

## 02 角色规范说明图

```text
Create one character specification sheet for a stable minimalist hand-drawn diagram persona.

Purpose:
This sheet is for user confirmation, QA, and correction. It is not the primary generation anchor and should not be overcrowded.

Confirmed creator persona:
{角色主锚图摘要：发型、眼镜/配饰、服装、体态、气质、点缀色}

Visual style:
Pure white background. Beautiful minimalist black hand-drawn line art. Slightly wobbly but clean pen lines. Clean hand-drawn panels. Sparse red/orange/blue accents only where useful.

Sheet layout:
1. One large main persona labeled "主识别".
2. "必须保留": 4-6 callouts for identity anchors.
3. "不要这样": 4-6 forbidden mini sketches with red X marks, such as wrong outfit, wrong glasses/accessory, childlike version, business suit, realistic photo look, cute mascot look.
4. "常用道具": {职业道具}
5. "配色": black, dark gray, white, personal accent color, optional secondary color.
6. "使用建议": short labels only.

Important:
Every mini persona in this sheet must still preserve the identity anchors. If a small sample cannot keep the anchors, remove it rather than making a misleading reference.

Chinese labels:
Use short, readable handwritten Chinese labels. No long paragraphs.

Avoid:
Do not make the sheet too dense. Do not create many tiny inconsistent faces. Do not create commercial brand manual style, PPT style, glossy rendering, chibi, or realistic photo.
```

## 03 动作 / 表情 / 小比例场景扩展图

```text
Create one action, expression, and small-scene extension sheet for a stable minimalist hand-drawn diagram persona.

Purpose:
This sheet is used when future diagrams need complex actions, expressions, or small characters inside spacious article illustrations. It must preserve the creator identity even when the character occupies only 10%-20% of the scene.

Confirmed creator persona:
{角色主锚图摘要：发型、眼镜/配饰、服装、体态、气质、点缀色}

Visual style:
Pure white background. Beautiful minimalist black hand-drawn line art. Slightly wobbly but clean pen lines. Lots of white space. Sparse accent colors only on the required identity accents, arrows, and emphasis marks.

Sheet layout:
1. Top anchor strip: one medium bust labeled "统一锚点".
2. "小比例图解角色": 6-10 small full-body scene poses. Every pose must preserve identity anchors.
3. "常用动作": 4-8 medium action samples.
4. "主角 + Agent 协作": 4-6 small scenes where the creator assigns, reviews, corrects, or receives work from execution Agents.
5. "表情参考": 4-6 bust expressions.

Domain-specific override:
If the creator has a clear course, industry, or recurring content series, replace the generic pose list with scenes from that domain. The action sheet should feel made for this creator's real content, not a universal action library.

Creator + Agent collaboration samples:
- 给执行 Agent 分配任务
- 执行 Agent 递回结果
- 执行 Agent 搬运知识卡
- 执行 Agent 把失败方案打叉
- 主角在白板前调度多个 Agents
- 主角批注 Agent 产出的草稿

Chinese labels:
Use short, readable handwritten Chinese labels only. Use "Agents" or "执行 Agent" if labels are needed. Do not write internal nicknames.

Avoid:
No inconsistent clothing colors. No missing required glasses/accessories. No childlike proportions. No business suit. No commercial poster. No PPT infographic. No realistic portrait. No dense layout.
```

## 内容图解通用 prompt

```text
Generate one standalone {aspect_ratio} Chinese visual diagram using the confirmed creator persona.

Character reference assets for this generation:
- Primary reference: {角色主锚图}
- Additional reference if needed: {动作/表情/小比例场景扩展图}
- Correction reference only if needed: {角色规范说明图}

Confirmed creator persona:
{角色档案摘要：发型、眼镜/配饰、服装、体态、气质、道具、点缀色}

Use case:
{长文配图 / 图文号知识卡 / 手机海报 / 方法拆解图 / 分镜故事图}

Visual mode:
{手绘插图模式 / 知识卡模式}

If knowledge card mode, card form:
{观点卡 / 路线图卡 / 白板讲解卡 / 行动工单卡 / 课程总览卡 / 章节封面卡 / 诊断评分卡 / 产品截图批注卡 / 立体沙盘卡 / 分镜知识卡 / or a custom card form designed for this content}

Visual DNA:
Pure white background. Beautiful minimalist black hand-drawn line art. Slightly wobbly but clean pen lines. Lots of clean empty space according to the chosen information level. Sparse red/orange/blue handwritten Chinese annotations. Refined creator IP plus clean absurd product-sketch feeling. No ugly rough doodle, no stiff business portrait, no gradients, no shadows, no paper texture, no complex background, no commercial vector style, no PPT look, no cute mascot poster, no children's illustration, no realistic interface reproduction.

Content brief:
- Core idea: {核心观点}
- Image title or main phrase: {图内标题}
- Required text on image: {图内文字}
- Must-preserve words: {必须保留的词}
- Flexible text: {可自由发挥的部分}

Structure type:
{Workflow / system close-up / before-after / role states / concept metaphor / method layers / route map / storyboard}

Main visual metaphor:
{主画面隐喻}

Creator persona action:
{角色动作。角色必须参与核心动作，不要站在旁边装饰。}

Supporting roles:
{Agents / 执行 Agent / 用户 / 失败案例 / 反馈来源 / 风险提示等。For knowledge cards about steps, workflows, methods, comparisons, cases, risks, or action checklists, include 2-6 execution Agents by default. Assign each Agent a concrete job such as carrying cards, testing a step, raising feedback, marking a failed case, handing back a result, or flagging a risk. Do not write internal nicknames on the image.}

Suggested elements:
{建议元素}

Information level:
{画面更空 / 讲清楚重点 / 内容更完整 / 完整海报}

Mode-specific composition:
- If visual mode is hand-drawn illustration mode: keep it spacious like an article illustration. Use one dominant metaphor or action. Even at higher information level, do not fill the full canvas like an infographic. If the creator persona is small in a big scene, preserve identity through hair silhouette, glasses/accessory, outfit, and body language.
- If visual mode is knowledge card mode: organize the image as a complete readable content card. Choose or invent a card form that fits the information structure and aspect ratio. The confirmed creator persona should act as the main explainer, guide, annotator, or dispatcher. Supporting Agents are default visual grammar for methods, steps, workflows, comparisons, cases, risks, and action checklists: use 2-6 Agents to execute, carry, test, fail, report, or flag parts of the content. Only omit them for pure quote cards, very minimal covers, or when the user explicitly asks for no Agents.

Color use:
Black for main line art and text. Orange for main flow/path/arrows. Red only for key warnings/problems/results. Blue only for secondary notes or feedback/system state.

Constraints:
One image explains the selected core idea. Keep text readable. Do not write unnecessary long paragraphs. Do not write the structure type on the image. If the image is a method / step / workflow / comparison / risk / action checklist knowledge card and there are no execution Agents or action metaphors, the result is incomplete and should be revised. Do not make it a formal PPT, course slide, commercial poster, or dense corporate infographic unless the selected use case is a phone poster and the user confirmed it. Do not copy prior examples or reuse known case compositions. Invent a fresh, strange-but-clear visual metaphor for this specific content. The creator persona must be recognizable and stable.
```

## PPT 演讲页面 prompt

```text
Generate one standalone 16:9 Chinese PPT presentation page using the confirmed creator persona.

This is PPT presentation mode, not a knowledge card and not an article illustration. The page must look like a real presentation slide while keeping a minimalist hand-drawn whiteboard style.

Character reference assets for this generation:
- Primary reference: {角色主锚图}
- Additional reference if needed: {动作/表情/小比例场景扩展图}
- Correction reference only if needed: {角色规范说明图}

Confirmed creator persona:
{角色档案摘要：发型、眼镜/配饰、服装、体态、气质、道具、点缀色}

Page card:
- Page number: {页码}
- Page type: {封面页 / 大判断页 / 模块页 / 标准页 / 场景页 / 时间线页 / 方法页 / 收束页 / 其他}
- Visual weight: {anchor / dense / breathing}
- Communication task: {沟通任务}
- Core idea: {核心观点}
- Page title: {图内标题}
- Required text: {图内文字}
- Text-to-image ratio: {图文比例}
- Main visual: {主视觉}
- Creator persona role: {IP 角色职责}
- Supporting Agents / people role: {辅助 Agent / 人物职责}
- Density: {页面密度}
- Continuity: {前后页衔接}

Visual DNA:
White or near-white background. Minimalist hand-drawn business whiteboard style. Stable PPT layout discipline. Clear hierarchy. Black and dark gray line art. Orange only for key emphasis, paths, buttons, or underlines. Blue only for structural links when needed. No gradients, no glossy corporate template, no tech neon style, no commercial poster feeling.

Typography:
Main title must be stable, bold, businesslike, and clear. Body text and labels should feel consistent. Handwritten text is allowed only as small annotations, not as the main information. Keep Chinese text readable.

Composition:
Make it a complete PPT page. Use grid, alignment, clear whitespace, and one communication task. Do not make it a dense infographic poster or a classroom handout. The creator persona must have a real page duty, such as presenting, pointing, observing, operating, or closing the talk. Do not place the persona as decoration.

Constraints:
No fake words, no unreadable small text, no random English unless explicitly requested. Do not overuse orange. Do not make every page high-density. Do not let the creator persona drift in age, clothes, hair, glasses/accessories, or vibe.
```

## 返修 prompt 模板

```text
Revise the provided image while preserving the same creator persona and the same core idea.

Reference priority:
1. Preserve the primary character anchor.
2. Use the action/expression/small-scene sheet for pose correction.
3. Use the specification sheet only for forbidden drift and QA correction.

Keep:
- Creator identity anchors: {保留锚点}
- Core idea: {核心观点}
- Use case and aspect ratio: {图类型和尺寸}
- Overall minimalist white hand-drawn diagram style

Change:
{本轮返修要求}

Text requirements:
Keep these exact Chinese words readable: {必须保留文字}
Remove or simplify: {要删减文字}
Use Agents, 执行 Agent, 用户, 执行者, 反馈来源, or 风险提示 where needed.

Avoid:
{禁区}
```
