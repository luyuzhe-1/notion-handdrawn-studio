# 提示词构建

用紧凑的完整描述代替大量重复形容词；中文或英文皆可。下面是构建槽位，不是固定输出格式，也不把全部槽位强行填满。

## 新图

先确定模式。有人物时使用下面的「人物造型基准」，再附当前主题的短动作描述；纯物件、装饰和 Logo 仍按各自参考构建，不套人物基准。不要把多篇参考文件串成一个不断加长的提示词。

### 人物造型基准

这是默认人物方向的可直接使用文本。用户没有要求改变画风时，跨场景沿用同一段；只修改主题、动作、构图、明确文字和背景。用户明确指定的体态、服装、身份或画风优先，不把此段当成固定角色模板。

```text
Draw a deliberately schematic black-and-white ink character in the quiet visual language of Notion website illustrations. Build the person from a few broad flat shapes: a roomy torso, sweeping curved sleeves and limbs, simple elongated lower-body shapes, and small plain feet. Silhouette and gesture carry the action. Elbows and knees are broad changes of direction within the shape. Hands are small flat palm shapes with only the thumb or grouped finger indication needed for the action. Hair is a quiet ink mass; the face has just a few small marks. Use clean, slightly irregular continuous contours, opaque white shapes and selective solid black shapes. Clothing interiors are mostly empty; add an interior line only when a contact or overlap would otherwise be unclear. Keep adult character proportions playfully abstract, the pose supported, and gaps between limbs readable. No anatomical modelling, garment construction detail, shading, texture or decorative flourishes.
```

主题段只补充人物是谁、做什么、与哪件物品接触、画面如何容纳主体。用动作信息扩充简单想法，不自行添加年龄质感、时装、面料、身体结构和摄影式描述。服装未指定时选便于组成完整大形的普通衣服；不要把宽袖、黑裤或某个发型规定为所有人物的身份。

接触动作写成可看见的证据，例如「粉笔尖接在正在形成的笔画末端」「壶嘴朝花盆，水线落入盆内」。保留解释动作必需的信息，不通过逐个描述关节与手指来追求真实性。文字逐字列出；不需要文字时写无文字。

构图按用途选择，说明关键部位完整、留白与白底／透明底。负向限制只补充当前主题的实际风险，不重复基准、堆叠风格同义词，或把历史错误逐一变成永久禁令。

### 图片输入与生成记录

新图与编辑分别遵守工具当前规则。若内置工具要求新图省略图片参数，查看参考后把观察转成文字；记录 `reference_mode: viewed_then_text`，不声称图片被传给了生成器。允许图片参考的工具才标明各图的风格参考角色。不得为了传参考而把全新场景伪装成编辑。

透明背景同时通过工具的 `transparent_background` 选项指定。不要使用不存在的内置参数，或把 CLI 的 quality／尺寸旗标当成工具选项。

保留实际完整提示词、参考 ID、输入方式、工具与每次输出。首次生成原样保留；后续编辑另存并分别评价。仅提示词任务交付完整文本，不调用生成工具。

## 编辑

先查看目标。说明“只改什么”，再列与此次修改相关的不变量。把风格参考与编辑目标分别标记；编辑透明图时保留透明通道。不要为修一个错误重新发明场景。

若用户要人物更抽象、柔和，明确允许重塑人物相关轮廓与局部比例，不变量写成“坐姿／抬手的动作意图、重心、手与道具的接触、主体布局”等。不要同时要求保留原有每一段肢体形状；若只获准删衣褶，则仍遵守该窄编辑范围。

## 小幅迭代

从真实成图指出一个缺陷，进行一次针对性编辑；没有明显问题就不增加生成次数。若同一问题仍在，交付当前结果及未解决项让用户决定。用户提出的新修改可开启新一轮。
