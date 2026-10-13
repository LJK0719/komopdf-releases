# komopdf 0.1.9

## 交互性能与光标修复 / Interaction performance and caret fixes

- 减少拖动、框选及调整文本框时的重复计算和不必要界面刷新；保留准确的最终位置与一次提交。
- 修复原位编辑越到段尾光标越偏、最后两个位置无法准确点击的问题。未修改时，点击、光标和选区使用原 PDF 的真实字符位置。
- 新输入继承插入点的字体和字距；输入法组合、草稿修改与撤销之间正确切换光标布局。
- 修复连续粗斜体/字体操作丢失字体面、保存重开后同款补字被误判的问题；兼容更多原字体名称格式。
- 编辑时保持仍可见的活动页，避免工具栏布局变化把编辑对象切到另一页。
- 保留自动系统字体、源字形与间距、文本容器隐藏内容恢复及图片/路径变换。

- Reduce repeated calculations and unnecessary UI work during selection, moving and text-frame resizing while committing the final position once.
- Fix inaccurate inline caret placement near the end of source text. Pristine clicks, caret and selection use the original PDF character geometry.
- Preserve the insertion point's font and spacing, with correct caret transitions for drafts, undo and IME composition.
- Preserve exact faces during consecutive formatting operations and match missing-glyph completion to actual embedded font metadata after reopening.
- Keep a still-visible editing page active across toolbar/layout changes.

## 下载与说明 / Download and notes

Windows x64，Windows 10 22H2 或更新版本，包含完整离线运行时与第三方许可。本次不提供新的 macOS 安装包。

非 AI PDF 功能继续免费、无需登录。系统商业字体不随产品分发；网页本地字体仍遵循浏览器授权。账户、积分、订阅与历史规则不变。

GitHub's automatic source archives contain this release repository's public documentation, not the private desktop source or an installer.
