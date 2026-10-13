# komopdf 0.1.8

## 文本编辑与字体修复 / Text editing and font fixes

- 文本选择只显示一个真实文本框；选中和悬停高亮不再跟随过大的外扩框。
- 双击直接在原位置编辑，不再弹出带描边、阴影的浮出式编辑框。未修改时保留原 PDF 字形；取消或无修改完成不改变文档。
- Windows 客户端自动提供系统字体，包括宋体、新宋体和已安装的用户字体，不再要求先手动导入。字体目录显示真实名称和别名，字节按首次使用加载。
- 续写保留原字体、字号和字距；原 PDF 字体子集缺字时使用同款完整字体补齐新增部分，不静默替换整段。保存重开后仍可继续编辑。
- 保留 0.1.7 的文本容器调整、隐藏行恢复，以及图片和路径缩放行为。

- Text selection and hover use one actual text frame instead of overlapping padded outlines.
- Double-click editing stays in place without a floating bordered panel. Unchanged PDF glyphs remain visible; cancelling or finishing without edits leaves the document untouched.
- Windows automatically lists installed system and user fonts by their real names and aliases, loading each face on first use.
- Content edits retain the source font and spacing. Missing subset glyphs use a matching complete font for the added text rather than replacing the original paragraph. Saved PDFs remain editable after reopening.

## 下载与说明 / Download and notes

Windows x64，Windows 10 22H2 或更新版本；提供完整离线运行时及第三方许可。本次没有新增 macOS 安装包。

系统字体不随产品分发。若原字体或同款完整字体不可用，需明确选择替代字体；网页本地字体访问仍遵循浏览器授权。

非 AI PDF 功能继续免费、无需登录。账户、积分、订阅和历史对话规则不变。

GitHub's automatic source archives contain this release repository's public documentation, not the private desktop source or an installer.
